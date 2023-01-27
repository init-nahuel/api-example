# api-example

API example for projects, it can be use as template.

You can start the project with `nodemon` making the server `http://localhost:3333/` listen to any modifications to the files on the project folder using:

```bash
# Run project
yarn start:dev
```

If you want to deploy the application, you just have to run:

```bash
# Build project
yarn build

# Start the built server.js
yarn start:prod
```

- `yarn build`: Will run the `tsc` command to compile `.ts` files into `.js` files inside the folder that was defined on `tsconfig.json` (`dist` folder).
- `yarn start:prod`: Will start the built `server.js` file inside the `dist` folder.
- `yarn start:dev`: Will start the project with `nodemon` (who will run `ts-node`), making the server listen to any modifications to the files on the poject folder.
