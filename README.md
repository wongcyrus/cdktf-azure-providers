# cdktf-azure-providers

This package includes:
```
    "azurerm@~>4.0.0",
    "azuread@~>3.0.0",
    "random@~>3.6.2",
    "null@~>3.2.4",
    "external@~>2.3.4",
    "archive@~>2.7.0",
    "http@~>3.4.4",
    "template@~>2.2.0",
    "local@~>2.5.2",
    "time@~>0.12.0"
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



