##PasteOptions
Represents the paste special options.
## PasteOptions class
Represents the paste special options.
```javascript
class PasteOptions;
```
## Constructors
| Name | Description |
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
