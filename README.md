# Delete-Metadata-Using-SalesforceCLI

## how to use

- open DeployChanges in vscode (one level down from the repo)
- add types you want to delete to destructuveChanges.xml

e.g.
```xml
<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
<Package xmlns="http://soap.sforce.com/2006/04/metadata">
    <types>
        <members>MyApexClass</members>
        <members>MyApexClass2</members>
        <name>ApexClass</name>
    </types>
    <types>
        <members>MyApexPage</members>
        <name>ApexPage</name>
    </types>
</Package>
```
- use ```cmd + shift + b```
- select ```SFDX: Delete Metadata```
- enter the username of the org you want to delete the metadata from
- hit enter.