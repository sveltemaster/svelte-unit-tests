# setup
Run `npm install --save-dev svelte-jester jest babel-jest @testing-library/svelte @babel/preset-env @babel/core`     

# Add this to package.json
### Add this to your scripts:     
"test": "jest src"
### Add this at the bottom
```
"jest": {
    "bail": false,
    "moduleFileExtensions": [
      "js",
      "svelte"
    ],
    "transform": {
      "^.+\\.js$": "babel-jest",
      "^.+\\.svelte$": "svelte-jester"
    },
    "verbose": true
  },
  "babel": {
    "presets": [
      [
        "@babel/preset-env",
        {
          "targets": {
            "node": "current"
          }
        }
      ]
    ]
  }
```