# cdktf-azure-providers

This package includes:
```
    "azurerm@~>4.40.0",
    "azuread@~>3.5.0",
    "random@~>3.7.2",
    "null@~>3.2.4",
    "external@~>2.3.5",
    "archive@~>2.7.1",
    "http@~>3.5.0",
    "template@~>2.2.0",
    "local@~>2.5.3",
    "time@~>0.13.1"
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



