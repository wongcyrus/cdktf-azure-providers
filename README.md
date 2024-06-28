# cdktf-azure-providers

This package includes:
```
    "azurerm@~>3.109.0",
    "azuread@~>2.52.0",
    "random@~>3.6.2",
    "null@~>3.2.2",
    "external@~>2.3.3",
    "archive@~>2.4.2",
    "http@~>3.4.3",
    "template@~>2.2.0",
    "local@~>2.5.1",
    "time@~>0.11.2"
 ```

Install CDKTF and login npm
```
npm install --global cdktf-cli@latest
npm adduser
```

To publish new version, you need to compile ts in .gen to js.
```
npm run get
npm run build
npm publish
```



