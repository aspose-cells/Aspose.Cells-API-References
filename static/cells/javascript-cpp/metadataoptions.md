##MetadataOptions
Represents the options of loading metadata of the file.
## MetadataOptions class
Represents the options of loading metadata of the file.
```javascript
class MetadataOptions;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(MetadataType)](#constructor-metadatatype-)| Creates an options of loading the metadata. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [metadataType](#metadataType--)| MetadataType | Readonly. Gets and sets the type of the metadata which is loading. |
| [password](#password--)| string | Represents Workbook file encryption password. |
| [keyLength](#keyLength--)| number | The key length. |
### constructor(MetadataType) {#constructor-metadatatype-}
Creates an options of loading the metadata.
```javascript
constructor(metadataType: MetadataType);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| metadataType | [MetadataType](../metadatatype/) | The type of metadata. |
### metadataType {#metadataType--}
Readonly. Gets and sets the type of the metadata which is loading.
```javascript
metadataType : MetadataType;
```
### password {#password--}
Represents Workbook file encryption password.
```javascript
password : string;
```
### keyLength {#keyLength--}
The key length.
```javascript
keyLength : number;
```
