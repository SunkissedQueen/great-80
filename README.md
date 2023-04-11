## Create rails app
- $ rails new great_80 --skip-javascript -d postgresql -T
- $ cd great_80
- $ ga .
- $ gcmsg "initial commit with shakapacker"
- $ git branch -M main
- $ git remote add origin https://github.com/SunkissedQueen/great-80.git
- $ git push -u origin main
- $ code .

## add shakapacker
- $ bundle add shakapacker --strict
- $ ./bin/bundle install
- $ ./bin/rails webpacker:install
- Remove webpack-dev-server from dependencies
- $ yarn add --dev webpack-dev-server
- Add preset for react on package.json > babels
```json
  "babel": {
    "presets": [
      "./node_modules/shakapacker/package/babel/preset.js",
      "@babel/preset-react"
    ]
  }
```