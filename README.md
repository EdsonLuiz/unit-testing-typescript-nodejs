# unit-testing-typescript-nodejs
Practice tests in typescript

## Start adding packages
```bash
npm i -D typescript ts-node @types/node jest ts-jest @types/jest
```

## Configure Jest to use typescript
```javascript
// jest.config.js
module.exports = {
  roots: ['<rootDir>/src'],
  transform: {
    '^.+\\.tsx?$': 'ts-jest'
  },
  testRegex: '(/__test__/.*|(\\.|/)(test|spec))\\.[jt]sx?$',
  moduleFileExtensions: ['ts', 'tsx', 'js', 'jsx', 'json', 'node'],
  verbose: true
}
```