##MetadataOptions
Represents the options of loading metadata of the file.
## MetadataOptions class
Represents the options of loading metadata of the file.
```javascript
class MetadataOptions;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(MetadataType)](#constructor-metadatatype-)| Creates an options of loading the metadata. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [metadataType](#metadataType--)| MetadataType | Readonly. Gets and sets the type of the metadata which is loading. |
| [password](#password--)| string | Represents Workbook file encryption password. |
| [keyLength](#keyLength--)| number | The key length. |
## Methods
| Method | Description |
| --- | --- |
| [getMetadataType()](#getMetadataType--)| <b>@deprecated.</b> Please use the 'metadataType' property instead. Gets and sets the type of the metadata which is loading. |
| [getPassword()](#getPassword--)| <b>@deprecated.</b> Please use the 'password' property instead. Represents Workbook file encryption password. |
| [setPassword(string)](#setPassword-string-)| <b>@deprecated.</b> Please use the 'password' property instead. Represents Workbook file encryption password. |
| [getKeyLength()](#getKeyLength--)| <b>@deprecated.</b> Please use the 'keyLength' property instead. The key length. |
| [setKeyLength(number)](#setKeyLength-number-)| <b>@deprecated.</b> Please use the 'keyLength' property instead. The key length. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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
### getMetadataType() {#getMetadataType--}
```javascript
getMetadataType() : MetadataType;
```
**Returns**
[MetadataType](../metadatatype/)
### getPassword() {#getPassword--}
```javascript
getPassword() : string;
```
### setPassword(string) {#setPassword-string-}
```javascript
setPassword(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getKeyLength() {#getKeyLength--}
```javascript
getKeyLength() : number;
```
### setKeyLength(number) {#setKeyLength-number-}
```javascript
setKeyLength(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
