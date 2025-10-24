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
| [getAuthor()](#getAuthor--)| <b>@deprecated.</b> Please use the 'author' property instead. Gets and sets the author. |
| [setAuthor(string)](#setAuthor-string-)| <b>@deprecated.</b> Please use the 'author' property instead. Gets and sets the author. |
| [getRecommendReadOnly()](#getRecommendReadOnly--)| <b>@deprecated.</b> Please use the 'recommendReadOnly' property instead. Indicates if the Read Only Recommended option is selected. |
| [setRecommendReadOnly(boolean)](#setRecommendReadOnly-boolean-)| <b>@deprecated.</b> Please use the 'recommendReadOnly' property instead. Indicates if the Read Only Recommended option is selected. |
| [isWriteProtected()](#isWriteProtected--)| <b>@deprecated.</b> Please use the 'isWriteProtected' property instead. Indicates whether this workbook is write protected. |
| [getPassword()](#getPassword--)| <b>@deprecated.</b> Please use the 'password' property instead. Sets the protected password to modify the file. |
| [setPassword(string)](#setPassword-string-)| <b>@deprecated.</b> Please use the 'password' property instead. Sets the protected password to modify the file. |
| [validatePassword(string)](#validatePassword-string-)| Returns true if the specified password is the same as the write-protection password the file was protected with. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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
### getAuthor() {#getAuthor--}
```javascript
getAuthor() : string;
```
### setAuthor(string) {#setAuthor-string-}
```javascript
setAuthor(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getRecommendReadOnly() {#getRecommendReadOnly--}
```javascript
getRecommendReadOnly() : boolean;
```
### setRecommendReadOnly(boolean) {#setRecommendReadOnly-boolean-}
```javascript
setRecommendReadOnly(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isWriteProtected() {#isWriteProtected--}
```javascript
isWriteProtected() : boolean;
```
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
### validatePassword(string) {#validatePassword-string-}
Returns true if the specified password is the same as the write-protection password the file was protected with.
```javascript
validatePassword(password: string) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | string | The specified password. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
