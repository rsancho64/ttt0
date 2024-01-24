## fix cdigital-envelope-routinesunsupported error

https://stackoverflow.com/questions/69692842/error-message-error0308010cdigital-envelope-routinesunsupported
1094 hits
In your package.json: change this line

- "start": "react-scripts start"

to

- "start": "react-scripts --openssl-legacy-provider start"

