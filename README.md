# Modified react-scripts to include customisable homepage

Use by setting a default homepage value and alternates in snek_case, ex:

```json
{
	"homepage_gh": "https://oxfordunichess.github.io/oucc-frontend/",
  	"homepage": "http://users.ox.ac.uk/~chess/",
}
```

Modify by using a cli argument in react-scripts


```json
  "scripts": {
    "start": "react-scripts start",
    "seo": "react-snapshot",
    "build": "react-scripts build",
    "test": "react-scripts test",
    "eject": "react-scripts eject",
    "predeploy": "yarn build --homepage gh",
    "deploy": "gh-pages -d build",
    "deploy-sso": "gh-pages -d build -b sso"
  },
  ```