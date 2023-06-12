# firebase

## basic
npm install -g firebase-tools
firebase login
firebase init

## set hosting
```
{
  "hosting": {
    "site": "nexus9",
    "public": "public",
  }
}
```

## deploy
```
firebase deploy --only hosting:nexus9
```