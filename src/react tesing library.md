# react testing library

1. new react myapp

2. install pacakges
```
yarn add --dev jest
yarn add --dev babel-jest @babel/core @babel/preset-env @babel/preset-react
yarn add --dev jest-environment-jsdom
yarn add --dev @testing-library/react 
```

3. jest config
```
/** @type {import('jest').Config} */
const config = {
  testEnvironment: 'jsdom',
  //setupFiles: ['<rootDir>/setupJest.js'],
};

module.exports = config;
```

4. babel config
```
module.exports = {
  presets: [
    '@babel/preset-env',
    ['@babel/preset-react', {runtime: 'automatic'}],
  ],
};
```

5. test component
```
const Hello = () => <h1 data-testid="nxHello">Hello React</h1>

export default Hello
```

```
import { render } from '@testing-library/react'
import Hello from './Hello'

test('can render component', async () => {
  const wrapper = render(<Hello />)

  const el = wrapper.getByTestId('nxHello')
  expect(el.tagName).toBe('H1')
})
```

6. npx jest --watchAll
