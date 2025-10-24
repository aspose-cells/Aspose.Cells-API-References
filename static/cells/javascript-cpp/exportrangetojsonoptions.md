##ExportRangeToJsonOptions
Indicates the options that exporting range to json.
## ExportRangeToJsonOptions class
Indicates the options that exporting range to json.
```javascript
class ExportRangeToJsonOptions;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [hasHeaderRow](#hasHeaderRow--)| boolean | Indicates whether the range contains header row. |
| [exportAsString](#exportAsString--)| boolean | Exports the string value of the cells to json. |
| [exportEmptyCells](#exportEmptyCells--)| boolean | Indicates whether exporting empty cells as null. |
| [indent](#indent--)| string | Indicates the indent. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### hasHeaderRow {#hasHeaderRow--}
Indicates whether the range contains header row.
```javascript
hasHeaderRow : boolean;
```
### exportAsString {#exportAsString--}
Exports the string value of the cells to json.
```javascript
exportAsString : boolean;
```
### exportEmptyCells {#exportEmptyCells--}
Indicates whether exporting empty cells as null.
```javascript
exportEmptyCells : boolean;
```
### indent {#indent--}
Indicates the indent.
```javascript
indent : string;
```
**Remarks**
If the indent is null or empty, the exported json is not formatted.
