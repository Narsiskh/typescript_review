# typescript_review
## Benefits of TypeScript
1. Static typing:
TypeScript is JavaScript with Type Checking.
2. Code completion 
3. Refactoring
4. Shorthand notations

## Drawbacks
1. Compilation
- Transpilation :
.ts --> compiler --> .js
2. Discipline in coding
- TS : Medium to large projects
- JS : Simple projects 

## TS Program
- By typing a colon followed by the type of variable we can annotate or explain a variable. 
```typescript
let age: number = 20
```

## Configuring the TypeScript Compiler
```
tsc --init
```
```
Created a new tsconfig.json with:                                                              
                                                                                            
                                                                                           
  target: es2016
  module: commonjs
  strict: true
  esModuleInterop: true
  skipLibCheck: true
  forceConsistentCasingInFileNames: true

```
### tsconfig.json
1.  "target": "es2016" : Specifies the version of JS that the TS compiler is going to generate.
2. "module": "commonjs" : Specifies the directory that contains our source files.
3.  "outDir": "./"  : Specifies the directory that will contain our JS files.
4. "outDir": "./dist" : When we compile our code using the TS compiler our JS files are going to be stored in dist or distributable folder 
5.  "removeComments": true : If we enable this, the TS compiler is going to remove all the comments that we add in our TS code so the generated JS code is going to be shorter
6.  "noEmitOnError": true : By default when we compile our code even if we have errors in our code the TS compiler will still generate JS files. The best option is to always enable this setting. 