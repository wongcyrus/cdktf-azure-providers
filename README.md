# CDK Terrain Azure providers

This package contains CDK Terrain bindings for a pinned set of Terraform
providers used by the Azure construct libraries in this organization.

The npm package retains the historical `cdktf-azure-providers` name for
compatibility, but version `0.1.0` and later use CDK Terrain (`cdktn`) and do
not depend on the deprecated CDK for Terraform framework.

Provider versions:
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

## Development

Node.js 22.19 or newer is required.
Generating and compiling the AzureRM bindings requires a memory-constrained
Node.js build process; use a development environment with at least 12 GB RAM.

```
npm install
npm run get
npm test
```

Provider bindings are generated into `.gen` and included in the npm package.
The generated directory is intentionally not committed.

To publish a new version:

```
npm run build
npm pack --dry-run
npm publish
```

