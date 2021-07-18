## Node.js API with typescript from scratch
#### How to create a Node.js Rest Api using Typescript from scratch

## Dependences
- Typescript
- Express
- TypeORM
- SQLite3

### First Steps

------------

1.  #### Installing dependences

	- Start a node project: `npm init -y`

	- Install Typescript dependences: `npm i -D typescript ts-node`

	- Install Nodemon dependence: `npm i -D nodemon`

	- Install Express and TypeORM dependences `npm i express typeorm sqlite3`

	- Install Node Type Safe to Typescript  `npm install -D @types/node @types/express`

	- Start a Typescript Project: `npx tsc –init`

	- Create `.gitignore` file.

	- Add `node_modules` into `.gitignore` file.

2. #### Preparing the running scripts
	- Add `"start": "ts-node app.ts"` and `"start:dev": "nodemon app.ts"` to your scripts in `package.json` file.

3. #### Starting the project

	- Create `app.ts` file in your project root.

	- Import express in `app.ts` file `import express from 'express'`

	- To create a basic Rest server using Express:
```javascript
import express from 'express'
const port = 3000
const app = express()
app.listen(port, () => {
    console.log(`Server listening on port ${port}`)
})
```

