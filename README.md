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
