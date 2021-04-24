# Synthetic Package

This package contains common 3PP libraires for testing static code analysis engines.

All libraries are `*.resource` files located in the static resources folder:
```
 force-app/main/default/staticresources
```

Normally, each associated metadata file `*.resource-meta.xml` declares the mime-type of the resource. However, this mime-type is not reliable because it is not validated during upload, and is currently ignored at runtime. Therefore, we have introduced intentional errors to complicate the detection by the engines. 


| File | Declared Mime-Type | Description |
| --- | --- | --- |
| `archive.resource` | `aplication/zip` (intentional typo) |  zip file containing a large collection of 3PP libraires, mime-type |
| `jquery.resource` | `image/png` | zip file containing jQuery 1.12.1 |
| `jquery331.resource` | `text/plain` | text file containing jQuery 3.3.1 |
| `salesforce.resource` | `application/javascript` | binary file containing the Salesforce logo in PNG format |



