## Description:

Both "expo prebuild" and "expo run:android" commands fail due to invalid URL string

## How to reproduce:

1. Open the terminal and run the following:

`npx create-expo-app my-project`

2. Enter the directory:

`cd my-project`

3. Run one of the following commands:

`npx expo prebuild`

or


`npx expo run:android`

The result looks like this:
```
Could not parse JSON returned from "npm view expo-template-bare-minimum@sdk-51 dist.tarball --json".

https://registry.npmjs.org/expo-template-bare-minimum/-/expo-template-bare-minimum-51.0.26.tgz

Error: Unexpected token 'h', "https://re"... is not valid JSON
✖ Failed to create the native directories
You may want to delete the ./ios and/or ./android directories before trying again.
```
