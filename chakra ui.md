# Chakra UI

### 1. Install packages

```
npm i @chakra-ui/react @emotion/react @emotion/styled framer-motion
```

### 2. Import Provider

```js
import { ChakraProvider } from '@chakra-ui/react'

<ChakraProvider>
    <TheRestOfYourApplication />
</ChakraProvider>
```

### 3. Try an example 

```jsx
import { Button, ButtonGroup } from '@chakra-ui/react'

<Stack spacing={4} direction='row' align='center'>
  <Button colorScheme='teal' size='xs'>
    Button
  </Button>
  <Button colorScheme='teal' size='sm'>
    Button
  </Button>
  <Button colorScheme='teal' size='md'>
    Button
  </Button>
  <Button colorScheme='teal' size='lg'>
    Button
  </Button>
</Stack>
```