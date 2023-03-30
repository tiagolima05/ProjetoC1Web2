# Arquivo de documentação

## Instalações

Instale o typescript:
npm install typescript --save-dev


Crie um arquivo tsconfig.json na raiz do seu projeto e configure as opções necessárias para o TypeScript:

{
  "compilerOptions": {
    "target": "es6",
    "module": "commonjs",
    "outDir": "./dist",
    "esModuleInterop": true,
    "sourceMap": true
  },
  "include": ["src/**/*"],
  "exclude": ["node_modules", "**/*.spec.ts"]
}


Se você preferir não instalar o ts-node globalmente, pode instalá-lo localmente em seu projeto usando o comando npm install --save-dev ts-node. Em seguida, você precisará modificar o comando npm run dev em seu package.json:

"dev": "set NODE_ENV=dev&&nodemon ./src/server.ts",

## Rodando o projeto

Para transpilar o projeto, rode o comando tsc

Para rodar o projeto como typescript apenas, execute o comando: npm run dev
