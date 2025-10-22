##AbstractLowCodeProtectionProvider
Implementation to provide protection settings
## AbstractLowCodeProtectionProvider class
Implementation to provide protection settings
```javascript
class AbstractLowCodeProtectionProvider;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Methods
| Method | Description |
| --- | --- |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getOpenPassword()](#getOpenPassword--)| Gets the password to open spread sheet file. |
| [getWritePassword()](#getWritePassword--)| Gets the password to modify spread sheet file. |
| [getWorkbookPassword()](#getWorkbookPassword--)| Gets the password to protect the workbook with specified protection type. |
| [getWorkbookProtectionType()](#getWorkbookProtectionType--)| Gets the protection type to protect the workbook. |
| [getWorksheetPassword(string)](#getWorksheetPassword-string-)| Gets the password to protect the specified worksheet. |
| [getWorksheetProtectionType(string)](#getWorksheetProtectionType-string-)| Gets the protection type to protect the specified worksheet. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### getOpenPassword() {#getOpenPassword--}
Gets the password to open spread sheet file.
```javascript
getOpenPassword() : string;
```
**Returns**
Password to open spread sheet file. Empty means no protection for openning the filel.
### getWritePassword() {#getWritePassword--}
Gets the password to modify spread sheet file.
```javascript
getWritePassword() : string;
```
**Returns**
Password to modify the spread sheet file. Empty means no protection for modifying the file.
### getWorkbookPassword() {#getWorkbookPassword--}
Gets the password to protect the workbook with specified protection type.
```javascript
getWorkbookPassword() : string;
```
**Returns**
Password to protect the workbook.
### getWorkbookProtectionType() {#getWorkbookProtectionType--}
Gets the protection type to protect the workbook.
```javascript
getWorkbookProtectionType() : ProtectionType;
```
**Returns**
Protection type to protect the workbook. [ProtectionType.None](../protectiontype.none/) means no protection for the workbook.
### getWorksheetPassword(string) {#getWorksheetPassword-string-}
Gets the password to protect the specified worksheet.
```javascript
getWorksheetPassword(sheetName: string) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | string |  |
**Returns**
Password to protect the specified worksheet.
### getWorksheetProtectionType(string) {#getWorksheetProtectionType-string-}
Gets the protection type to protect the specified worksheet.
```javascript
getWorksheetProtectionType(sheetName: string) : ProtectionType;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | string |  |
**Returns**
Protection type to protect the specified worksheet. [ProtectionType.None](../protectiontype.none/) means no protection for the worksheet.
