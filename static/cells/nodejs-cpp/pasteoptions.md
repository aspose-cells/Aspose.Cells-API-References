##PasteOptions
Represents the paste special options.
## PasteOptions class
Represents the paste special options.
```javascript
class PasteOptions;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [pasteType](#pasteType--)| PasteType | The paste special type. |
| [skipBlanks](#skipBlanks--)| boolean | Indicates whether skips blank cells. |
| [keepOldTables](#keepOldTables--)| boolean | Keeps the tables in the destination range. |
| [onlyVisibleCells](#onlyVisibleCells--)| boolean | True means only copying visible cells. |
| [transpose](#transpose--)| boolean | True to transpose rows and columns when the range is pasted. The default value is False. |
| [operationType](#operationType--)| PasteOperationType | Gets and sets the operation type when pasting range. |
| [ignoreLinksToOriginalFile](#ignoreLinksToOriginalFile--)| boolean | Ingore links to the original file. |
## Methods
| Method | Description |
| --- | --- |
| [getPasteType()](#getPasteType--)| <b>@deprecated.</b> Please use the 'pasteType' property instead. The paste special type. |
| [setPasteType(PasteType)](#setPasteType-pastetype-)| <b>@deprecated.</b> Please use the 'pasteType' property instead. The paste special type. |
| [getSkipBlanks()](#getSkipBlanks--)| <b>@deprecated.</b> Please use the 'skipBlanks' property instead. Indicates whether skips blank cells. |
| [setSkipBlanks(boolean)](#setSkipBlanks-boolean-)| <b>@deprecated.</b> Please use the 'skipBlanks' property instead. Indicates whether skips blank cells. |
| [getKeepOldTables()](#getKeepOldTables--)| <b>@deprecated.</b> Please use the 'keepOldTables' property instead. Keeps the tables in the destination range. |
| [setKeepOldTables(boolean)](#setKeepOldTables-boolean-)| <b>@deprecated.</b> Please use the 'keepOldTables' property instead. Keeps the tables in the destination range. |
| [getOnlyVisibleCells()](#getOnlyVisibleCells--)| <b>@deprecated.</b> Please use the 'onlyVisibleCells' property instead. True means only copying visible cells. |
| [setOnlyVisibleCells(boolean)](#setOnlyVisibleCells-boolean-)| <b>@deprecated.</b> Please use the 'onlyVisibleCells' property instead. True means only copying visible cells. |
| [getTranspose()](#getTranspose--)| <b>@deprecated.</b> Please use the 'transpose' property instead. True to transpose rows and columns when the range is pasted. The default value is False. |
| [setTranspose(boolean)](#setTranspose-boolean-)| <b>@deprecated.</b> Please use the 'transpose' property instead. True to transpose rows and columns when the range is pasted. The default value is False. |
| [getOperationType()](#getOperationType--)| <b>@deprecated.</b> Please use the 'operationType' property instead. Gets and sets the operation type when pasting range. |
| [setOperationType(PasteOperationType)](#setOperationType-pasteoperationtype-)| <b>@deprecated.</b> Please use the 'operationType' property instead. Gets and sets the operation type when pasting range. |
| [getIgnoreLinksToOriginalFile()](#getIgnoreLinksToOriginalFile--)| <b>@deprecated.</b> Please use the 'ignoreLinksToOriginalFile' property instead. Ingore links to the original file. |
| [setIgnoreLinksToOriginalFile(boolean)](#setIgnoreLinksToOriginalFile-boolean-)| <b>@deprecated.</b> Please use the 'ignoreLinksToOriginalFile' property instead. Ingore links to the original file. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### pasteType {#pasteType--}
The paste special type.
```javascript
pasteType : PasteType;
```
### skipBlanks {#skipBlanks--}
Indicates whether skips blank cells.
```javascript
skipBlanks : boolean;
```
### keepOldTables {#keepOldTables--}
Keeps the tables in the destination range.
```javascript
keepOldTables : boolean;
```
### onlyVisibleCells {#onlyVisibleCells--}
True means only copying visible cells.
```javascript
onlyVisibleCells : boolean;
```
### transpose {#transpose--}
True to transpose rows and columns when the range is pasted. The default value is False.
```javascript
transpose : boolean;
```
### operationType {#operationType--}
Gets and sets the operation type when pasting range.
```javascript
operationType : PasteOperationType;
```
### ignoreLinksToOriginalFile {#ignoreLinksToOriginalFile--}
Ingore links to the original file.
```javascript
ignoreLinksToOriginalFile : boolean;
```
### getPasteType() {#getPasteType--}
```javascript
getPasteType() : PasteType;
```
**Returns**
[PasteType](../pastetype/)
### setPasteType(PasteType) {#setPasteType-pastetype-}
```javascript
setPasteType(value: PasteType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PasteType](../pastetype/) | The value to set. |
### getSkipBlanks() {#getSkipBlanks--}
```javascript
getSkipBlanks() : boolean;
```
### setSkipBlanks(boolean) {#setSkipBlanks-boolean-}
```javascript
setSkipBlanks(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getKeepOldTables() {#getKeepOldTables--}
```javascript
getKeepOldTables() : boolean;
```
### setKeepOldTables(boolean) {#setKeepOldTables-boolean-}
```javascript
setKeepOldTables(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getOnlyVisibleCells() {#getOnlyVisibleCells--}
```javascript
getOnlyVisibleCells() : boolean;
```
### setOnlyVisibleCells(boolean) {#setOnlyVisibleCells-boolean-}
```javascript
setOnlyVisibleCells(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getTranspose() {#getTranspose--}
```javascript
getTranspose() : boolean;
```
### setTranspose(boolean) {#setTranspose-boolean-}
```javascript
setTranspose(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getOperationType() {#getOperationType--}
```javascript
getOperationType() : PasteOperationType;
```
**Returns**
[PasteOperationType](../pasteoperationtype/)
### setOperationType(PasteOperationType) {#setOperationType-pasteoperationtype-}
```javascript
setOperationType(value: PasteOperationType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PasteOperationType](../pasteoperationtype/) | The value to set. |
### getIgnoreLinksToOriginalFile() {#getIgnoreLinksToOriginalFile--}
```javascript
getIgnoreLinksToOriginalFile() : boolean;
```
### setIgnoreLinksToOriginalFile(boolean) {#setIgnoreLinksToOriginalFile-boolean-}
```javascript
setIgnoreLinksToOriginalFile(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
