# Initialize an Empty TypeScript Node.js Project

Follow these steps to set up a new TypeScript Node.js project.

## 1. Create a New Directory

mkdir node-app
cd node-app

## 2. Initialize the Node.js Project
npm init -y

## 3. Initialize TypeScript Configuration
npx tsc --init

## 4. Configure tsconfig.json
Go to the tsconfig.json file and set the outDir and rootDir options:
"outDir": "./dist",
"rootDir": "./src"

## 5. Create Your TypeScript File
Make a .ts file in the src directory and write your TypeScript code in it.

## 6. Compile TypeScript Code
After writing your TypeScript code, run:
tsc -b
This will compile your TypeScript code into JavaScript.

## 7. Run Compiled JavaScript
You can now run the compiled JavaScript file with:
node dist/index.js

## Optional: Smoother Development Experience
## 8. Install ts-node
To avoid compiling the code every time, install ts-node:
npm install ts-node --save-dev

## 9. Update package.json Scripts
Add the following scripts to your package.json:
"scripts": {
  "build": "tsc",
  "start": "node dist/index.js",
  "dev": "ts-node src/index.ts"
}

## 10. Run TypeScript Directly
For development, run your TypeScript code directly with:
npm run dev
