# Shareable TypeScript config for Angular projects

<p>
  <a href="https://travis-ci.org/github/Angular-RU/angular-tsconfig">
    <img src="https://travis-ci.org/Angular-RU/angular-tsconfig.svg?branch=master" />
  </a>
  <a href="https://badge.fury.io/js/%40angular-ru%2Ftsconfig">
    <img src="https://badge.fury.io/js/%40angular-ru%2Ftsconfig.svg" />
  </a>
</p>

### Quick start

```bash
$ npm install @angular-ru/tsconfig -D
```

Add to your `tsconfig.json`:

```json5
{
    extends: '@angular-ru/tsconfig',
    angularCompilerOptions: {
        // override shared angularCompilerOptions
        strictTemplates: true,
        disableTypeScriptVersionCheck: true
    },
    compilerOptions: {
        // override shared compilerOptions
        outDir: 'dist',
        target: 'es2018',
        lib: ['es2018'],
        typeRoots: ['./node_modules/@types']
    }
}
```

If you want to know which properties were inherited, you can do:

```bash
$ tsc --showConfig --project tsconfig.json
```
