## A Functional Chat for Real Mathematicians

This chat is the greatest chat ever.

It is written in PureScript, which is essentially Haskell that compiles to (unoptimized) javascript.

### Installation

```
git clone https://github.com/Joern314/monad-chat.git
cd monad-chat
npm install
```

### For Developers: VSCode

To setup VSCode for development in PureScript the extensions 
```
- Dhall Language Support
- PureScript IDE
- PureScript Language Support
- vscode-purty
```
are recommended. The configuration file `.vscode/settings.json` should make them work out of the box.

Similar extensions are available for emacs, vim, atom, ...

### Building

To build the code run the `build`-task in npm:
```
npm run build
```

### Installing new Modules

Javascript modules can be installed with
```
npm install --save
```

PureScript modules are added as dependencies in `spago.dhall`. They are installed with
`npm run postinstall` which is also triggered by `npm install`.
