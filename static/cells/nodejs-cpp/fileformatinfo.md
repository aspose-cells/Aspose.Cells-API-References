##FileFormatInfo
Contains data returned by FileFormatUtil..fileformatutil file format detection methods.
## FileFormatInfo class
Contains data returned by [FileFormatUtil](../fileformatutil/) file format detection methods.
```javascript
class FileFormatInfo;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [isProtectedByRMS](#isProtectedByRMS--)| boolean | Readonly. Gets whether the file is protected by Microsoft Rights Management Server. |
| [isEncrypted](#isEncrypted--)| boolean | Readonly. Returns true if the document is encrypted and requires a password to open. |
| [fileFormatType](#fileFormatType--)| FileFormatType | Readonly. Gets the detected file format. |
| [loadFormat](#loadFormat--)| LoadFormat | Readonly. Gets the detected load format. |
## Methods
| Method | Description |
| --- | --- |
| [isProtectedByRMS()](#isProtectedByRMS--)| <b>@deprecated.</b> Please use the 'isProtectedByRMS' property instead. Gets whether the file is protected by Microsoft Rights Management Server. |
| [isEncrypted()](#isEncrypted--)| <b>@deprecated.</b> Please use the 'isEncrypted' property instead. Returns true if the document is encrypted and requires a password to open. |
| [getFileFormatType()](#getFileFormatType--)| <b>@deprecated.</b> Please use the 'fileFormatType' property instead. Gets the detected file format. |
| [getLoadFormat()](#getLoadFormat--)| <b>@deprecated.</b> Please use the 'loadFormat' property instead. Gets the detected load format. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### isProtectedByRMS {#isProtectedByRMS--}
Readonly. Gets whether the file is protected by Microsoft Rights Management Server.
```javascript
isProtectedByRMS : boolean;
```
### isEncrypted {#isEncrypted--}
Readonly. Returns true if the document is encrypted and requires a password to open.
```javascript
isEncrypted : boolean;
```
### fileFormatType {#fileFormatType--}
Readonly. Gets the detected file format.
```javascript
fileFormatType : FileFormatType;
```
### loadFormat {#loadFormat--}
Readonly. Gets the detected load format.
```javascript
loadFormat : LoadFormat;
```
### isProtectedByRMS() {#isProtectedByRMS--}
```javascript
isProtectedByRMS() : boolean;
```
### isEncrypted() {#isEncrypted--}
```javascript
isEncrypted() : boolean;
```
### getFileFormatType() {#getFileFormatType--}
```javascript
getFileFormatType() : FileFormatType;
```
**Returns**
[FileFormatType](../fileformattype/)
### getLoadFormat() {#getLoadFormat--}
```javascript
getLoadFormat() : LoadFormat;
```
**Returns**
[LoadFormat](../loadformat/)
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
