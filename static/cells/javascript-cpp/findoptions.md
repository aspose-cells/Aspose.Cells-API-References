##FindOptions
Represents find options.
## FindOptions class
Represents find options.
```javascript
class FindOptions;
```
### Example
```javascript
const { Workbook, FindOptions, CellArea, LookInType } = AsposeCells;
//Instantiate the workbook object
var workbook = new Workbook(data);
//Get Cells collection
var cells = workbook.worksheets.get(0).cells;
//Instantiate FindOptions Object
var findOptions = new FindOptions();
//Create a Cells Area
var ca = new CellArea();
ca.startRow = 8;
ca.startColumn = 2;
ca.endRow = 17;
ca.endColumn = 13;
//Set cells area for find options
findOptions.setRange(ca);
//Set searching properties
findOptions.searchBackward = false;
findOptions.searchOrderByRows = true;
findOptions.lookInType = LookInType.Values;
//Find the cell with 0 value
var cell = cells.find(0, null, findOptions);
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [caseSensitive](#caseSensitive--)| boolean | Indicates if the searched string is case sensitive. |
| [lookAtType](#lookAtType--)| LookAtType | Look at type. |
| [isRangeSet](#isRangeSet--)| boolean | Readonly. Indicates whether the searched range is set. |
| [searchBackward](#searchBackward--)| boolean | Whether search backward for cells. |
| [searchOrderByRows](#searchOrderByRows--)| boolean | Indicates whether search order by rows or columns. |
| [lookInType](#lookInType--)| LookInType | Look in type. |
| [regexKey](#regexKey--)| boolean | Indicates whether the searched key is regex. If true the searched key will be taken as regex and parsed. Otherwise the key will be parsed according to the rules in ms excel. |
| [valueTypeSensitive](#valueTypeSensitive--)| boolean | Indicates whether searched cell value type should be same with the searched key. |
| [style](#style--)| Style | The format to search for. |
| [convertNumericData](#convertNumericData--)| boolean | Gets or sets a value that indicates whether converting the searched string value to numeric data. |
## Methods
| Method | Description |
| --- | --- |
| [getRange()](#getRange--)| Gets and sets the searched range. |
| [setRange(CellArea)](#setRange-cellarea-)| Sets the searched range. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### caseSensitive {#caseSensitive--}
Indicates if the searched string is case sensitive.
```javascript
caseSensitive : boolean;
```
### lookAtType {#lookAtType--}
Look at type.
```javascript
lookAtType : LookAtType;
```
**Remarks**
When [RegexKey](../regexkey/) is true and user has specified the exact rule for the regex, for performance consideration this property should be set as [LookAtType.EntireContent](../lookattype.entirecontent/). Otherwise we will refactor the search key to ensure it can be matched according to the specific type. For example, when the type is [LookAtType.Contains](../lookattype.contains/)(this is the default value for this property), we will add wildcards at the beginning and end of the search key automatically. In this case, the regular expressions will become more complex and the performance will also decrease.
### isRangeSet {#isRangeSet--}
Readonly. Indicates whether the searched range is set.
```javascript
isRangeSet : boolean;
```
### searchBackward {#searchBackward--}
Whether search backward for cells.
```javascript
searchBackward : boolean;
```
### searchOrderByRows {#searchOrderByRows--}
Indicates whether search order by rows or columns.
```javascript
searchOrderByRows : boolean;
```
### lookInType {#lookInType--}
Look in type.
```javascript
lookInType : LookInType;
```
### regexKey {#regexKey--}
Indicates whether the searched key is regex. If true the searched key will be taken as regex and parsed. Otherwise the key will be parsed according to the rules in ms excel.
```javascript
regexKey : boolean;
```
**Remarks**
Even though the search key has been specified as regex, it may be refactored according to specified [LookAtType](../lookattype/). For example, when the type is [LookAtType.Contains](../lookattype.contains/)(this is the default value for this options), wildcards will be added at the beginning and end of the search key automatically to ensure the match will be checked as "contains". In this case, the regular expressions will become more complex and the performance will also decrease. So, for performance consideration, if user has specified the exact rule for the regex, then there is no need to use [LookAtType](../lookattype/) as additional constraint and user may set it as [LookAtType.EntireContent](../lookattype.entirecontent/) to get better performance.
### valueTypeSensitive {#valueTypeSensitive--}
Indicates whether searched cell value type should be same with the searched key.
```javascript
valueTypeSensitive : boolean;
```
### style {#style--}
The format to search for.
```javascript
style : Style;
```
### convertNumericData {#convertNumericData--}
Gets or sets a value that indicates whether converting the searched string value to numeric data.
```javascript
convertNumericData : boolean;
```
### getRange() {#getRange--}
Gets and sets the searched range.
```javascript
getRange() : CellArea;
```
**Returns**
Returns the searched range.
### setRange(CellArea) {#setRange-cellarea-}
Sets the searched range.
```javascript
setRange(ca: CellArea) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../cellarea/) | the searched range. |
