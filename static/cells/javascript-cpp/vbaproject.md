##VbaProject
Represents the VBA project.
## VbaProject class
Represents the VBA project.
```javascript
class VbaProject;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [isValidSigned](#isValidSigned--)| boolean | Readonly. Indicates whether the signature of VBA project is valid or not. |
| [certRawData](#certRawData--)| Uint8Array | Readonly. Gets certificate raw data if this VBA project is signed. |
| [encoding](#encoding--)| EncodingType | Gets and sets the encoding of VBA project. |
| [name](#name--)| string | Gets and sets the name of the VBA project. |
| [isSigned](#isSigned--)| boolean | Readonly. Indicates whether VBAcode is signed or not. |
| [isProtected](#isProtected--)| boolean | Readonly. Indicates whether this VBA project is protected. |
| [islockedForViewing](#islockedForViewing--)| boolean | Readonly. Indicates whether this VBA project is locked for viewing. |
| [modules](#modules--)| VbaModuleCollection | Readonly. Gets all [VbaModule](../vbamodule/) objects. |
| [references](#references--)| VbaProjectReferenceCollection | Readonly. Gets all references of VBA project. |
## Methods
| Method | Description |
| --- | --- |
| [sign(DigitalSignature)](#sign-digitalsignature-)| Sign this VBA project by a DigitalSignature |
| [protect(boolean, string)](#protect-boolean-string-)| Protects or unprotects this VBA project. |
| [copy(VbaProject)](#copy-vbaproject-)| Copy VBA project from other file. |
| [validatePassword(string)](#validatePassword-string-)| Validates protection password. |
### isValidSigned {#isValidSigned--}
Readonly. Indicates whether the signature of VBA project is valid or not.
```javascript
isValidSigned : boolean;
```
### certRawData {#certRawData--}
Readonly. Gets certificate raw data if this VBA project is signed.
```javascript
certRawData : Uint8Array;
```
### encoding {#encoding--}
Gets and sets the encoding of VBA project.
```javascript
encoding : EncodingType;
```
### name {#name--}
Gets and sets the name of the VBA project.
```javascript
name : string;
```
### isSigned {#isSigned--}
Readonly. Indicates whether VBAcode is signed or not.
```javascript
isSigned : boolean;
```
### isProtected {#isProtected--}
Readonly. Indicates whether this VBA project is protected.
```javascript
isProtected : boolean;
```
### islockedForViewing {#islockedForViewing--}
Readonly. Indicates whether this VBA project is locked for viewing.
```javascript
islockedForViewing : boolean;
```
### modules {#modules--}
Readonly. Gets all [VbaModule](../vbamodule/) objects.
```javascript
modules : VbaModuleCollection;
```
### references {#references--}
Readonly. Gets all references of VBA project.
```javascript
references : VbaProjectReferenceCollection;
```
### sign(DigitalSignature) {#sign-digitalsignature-}
Sign this VBA project by a DigitalSignature
```javascript
sign(digitalSignature: DigitalSignature) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| digitalSignature | [DigitalSignature](../digitalsignature/) | DigitalSignature |
### protect(boolean, string) {#protect-boolean-string-}
Protects or unprotects this VBA project.
```javascript
protect(islockedForViewing: boolean, password: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| islockedForViewing | boolean | indicates whether locks project for viewing. |
| password | string | If the value is null, unprotects this VBA project, otherwise projects the this VBA project. |
**Remarks**
If islockedForViewing is true, the password could not be null.
### copy(VbaProject) {#copy-vbaproject-}
Copy VBA project from other file.
```javascript
copy(source: VbaProject) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [VbaProject](../vbaproject/) |  |
### validatePassword(string) {#validatePassword-string-}
Validates protection password.
```javascript
validatePassword(password: string) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | string | the password |
**Returns**
Whether password is the protection password of this VBA project
