create index.d.ts 

    declare namespace Guark {

    type EnvObject = { [Key: string]: string }

         const env = ():Promise<EnvObject> => {}
          /** Call exported Go functions. */
         const call = (funcName: string, args?: any): Promise<any> => {}
          /** Send desktop notification. */
         const notify = (message: string, args?: any): Promise<any> => {}
          /** Exit the app. */
         const exit = (): Promise<any> => {}
          /** Invoke a hook. */
         const hook = (name: string): Promise<any> => {}

    }

    export = Guark
    export as namespace Guark

# Guark React Template
Guark react app template.


## Install

Create new empty directory and cd to it, and run:
```bash
guark init --template react --mod github.com/username/appname
```

## Run dev app.

Run dev app with react hot reload:
```bash
guark run
```

## Build

```bash
guark build
```

## Bundle

```bash
guark bundle
```
