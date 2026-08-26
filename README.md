# CDK Terrain Azure providers

This package contains CDK Terrain bindings for a pinned set of Terraform
providers used by the Azure construct libraries in this organization.

The npm package retains the historical `cdktf-azure-providers` name for
compatibility, but version `0.1.0` and later use CDK Terrain (`cdktn`) and do
not depend on the deprecated CDK for Terraform framework.

Provider versions:
```
    "azurerm@~>5.2.0",
    "azuread@~>3.9.0",
    "random@~>3.9.0",
    "null@~>3.3.1",
    "external@~>2.4.1",
    "archive@~>2.8.0",
    "http@~>3.6.1",
    "local@~>2.9.0",
    "time@~>0.14.1"
 ```

## Development

Node.js 24.19 or newer is required.
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
