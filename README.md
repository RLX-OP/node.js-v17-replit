# node.js-v17-replit



Steps:

1. Execute this script **on the shell** to install node and configure npm.
```sh
npm init -y && npm i --save-dev node@17 && npm config set prefix=$(pwd)/node_modules/node && export PATH=$(pwd)/node_modules/node/bin:$PATH
```
## Or

```sh
npm install -D node@17
```

2. Create the [`.replit`](https://docs.repl.it/repls/dot-replit) to execute node from the shell instead of the console.
```
run = "npm start"
```

3. Make sure to add the start script in your package.json file
```js
  "scripts": {
    "start": "node ."
  }
```

## Or
In .replit file simply type
```
run = "npx node ."
```

4. (Optional) If you had packages like discord.js before, you need to re-install those packages
```
npm uninstall discord.js && npm install discord.js
```
