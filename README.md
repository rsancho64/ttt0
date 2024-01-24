## fix cdigital-envelope-routinesunsupported error

https://stackoverflow.com/questions/69692842/error-message-error0308010cdigital-envelope-routinesunsupported

- 1094 hits
- In your package.json: change this line

`"start": "react-scripts start",`

to

`"start": "react-scripts --openssl-legacy-provider start",`


## fix "react must be in scope when using jsx"

https://kinsta.com/knowledgebase/react-must-be-in-scope-when-using-jsx/

++ in `package.json`:

```json
"eslintConfig": {
    "extends": [
      "react-app",
      "react-app/jest"
    ],
    "rules": {
      "react/jsx-uses-react": "off",
      "react/react-in-jsx-scope": "off"
    }
  },
```
