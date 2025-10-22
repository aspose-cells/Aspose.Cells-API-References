##WriteProtection
Specifies write protection settings for a workbook.
## WriteProtection class
Specifies write protection settings for a workbook.
```javascript
class WriteProtection;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [author](#author--)| string | Gets and sets the author. |
| [recommendReadOnly](#recommendReadOnly--)| boolean | Indicates if the Read Only Recommended option is selected. |
| [isWriteProtected](#isWriteProtected--)| boolean | Readonly. Indicates whether this workbook is write protected. |
| [password](#password--)| string | Sets the protected password to modify the file. |
## Methods
| Method | Description |
| --- | --- |
| [validatePassword(string)](#validatePassword-string-)| Returns true if the specified password is the same as the write-protection password the file was protected with. |
### author {#author--}
Gets and sets the author.
```javascript
author : string;
```
### recommendReadOnly {#recommendReadOnly--}
Indicates if the Read Only Recommended option is selected.
```javascript
recommendReadOnly : boolean;
```
### isWriteProtected {#isWriteProtected--}
Readonly. Indicates whether this workbook is write protected.
```javascript
isWriteProtected : boolean;
```
### password {#password--}
Sets the protected password to modify the file.
```javascript
password : string;
```
### validatePassword(string) {#validatePassword-string-}
Returns true if the specified password is the same as the write-protection password the file was protected with.
```javascript
validatePassword(password: string) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | string | The specified password. |
