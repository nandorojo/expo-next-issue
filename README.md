# expo-next-issue

example repo for next issue with expo.

## How to run this example

```es6
git clone https://github.com/nandorojo/expo-next-issue
cd expo-next-issue
yarn
yarn next-dev
```

## How to recreate this example

**1. run this:**

```
expo init test
cd test
yarn add @expo/next-adapter react-native-paper
yarn expo-next
yarn next dev
```

**2. add this in pages/index.tsx:**

```es6
import * as React from 'react'
import { Button } from 'react-native-paper'

export default function Index() {
	return <Button>Hi, expo + next!</Button>
}
```

**3. open [http://localhost:3000](http://localhost:3000)**

## result

The app fails to compile. However, it works fine if I replace `Button` with a typical `Text` from `react-native`.

```es6
[ wait ]  compiling ...
[ error ] ./node_modules/@expo/vector-icons/build/vendor/react-native-vector-icons/Fonts/MaterialCommunityIcons.ttf 1:0
Module parse failed: Unexpected character '' (1:0)
You may need an appropriate loader to handle this file type, currently no loaders are configured to process this file. See https://webpack.js.org/concepts#loaders
(Source code omitted for this binary file)
ModuleParseError: Module parse failed: Unexpected character '' (1:0)
You may need an appropriate loader to handle this file type, currently no loaders are configured to process this file. See https://webpack.js.org/concepts#loaders
(Source code omitted for this binary file)
    at handleParseError (/Users/expo-next-test/node_modules/next/node_modules/webpack/lib/NormalModule.js:469:19)
    at /Users/expo-next-test/node_modules/next/node_modules/webpack/lib/NormalModule.js:503:5
    at /Users/expo-next-test/node_modules/next/node_modules/webpack/lib/NormalModule.js:358:12
    at /Users/expo-next-test/node_modules/loader-runner/lib/LoaderRunner.js:373:3
    at iterateNormalLoaders (/Users/expo-next-test/node_modules/loader-runner/lib/LoaderRunner.js:214:10)
    at /Users/expo-next-test/node_modules/loader-runner/lib/LoaderRunner.js:205:4
    at /Users/expo-next-test/node_modules/enhanced-resolve/lib/CachedInputFileSystem.js:85:15
    at processTicksAndRejections (internal/process/task_queues.js:75:11)
```
