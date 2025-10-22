##FileFormatInfo
Contains data returned by FileFormatUtil..fileformatutil file format detection methods.
## FileFormatInfo class
Contains data returned by [FileFormatUtil](../fileformatutil/) file format detection methods.
```javascript
class FileFormatInfo;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [isProtectedByRMS](#isProtectedByRMS--)| boolean | Readonly. Gets whether the file is protected by Microsoft Rights Management Server. |
| [isEncrypted](#isEncrypted--)| boolean | Readonly. Returns true if the document is encrypted and requires a password to open. |
| [fileFormatType](#fileFormatType--)| FileFormatType | Readonly. Gets the detected file format. |
| [loadFormat](#loadFormat--)| LoadFormat | Readonly. Gets the detected load format. |
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
