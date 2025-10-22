##ReferredArea
Represents a referred area by the formula.
## ReferredArea class
Represents a referred area by the formula.
```javascript
class ReferredArea;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [isExternalLink](#isExternalLink--)| boolean | Readonly. Indicates whether this is an external link. |
| [externalFileName](#externalFileName--)| string | Readonly. Get the external file name if this is an external reference. |
| [sheetName](#sheetName--)| string | Readonly. Indicates which sheet this reference is in. |
| [sheetNames](#sheetNames--)| string[] | Readonly. Names of all the worksheets this instance references to. |
| [isEntireRow](#isEntireRow--)| boolean | Readonly. Indicates whether this area contains all columns(entire row). |
| [isEntireColumn](#isEntireColumn--)| boolean | Readonly. Indicates whether this area contains all rows(entire column). |
| [isArea](#isArea--)| boolean | Readonly. Indicates whether this is an area. |
| [endColumn](#endColumn--)| number | Readonly. The end column of the area. |
| [startColumn](#startColumn--)| number | Readonly. The start column of the area. |
| [endRow](#endRow--)| number | Readonly. The end row of the area. |
| [startRow](#startRow--)| number | Readonly. The start row of the area. |
## Methods
| Method | Description |
| --- | --- |
| [getValues()](#getValues--)| Gets cell values in this area. |
| [getValues(boolean)](#getValues-boolean-)| Gets cell values in this area. |
| [getValue(number, number)](#getValue-number-number-)| Gets cell value with given offset from the top-left of this area. |
| [getValue(number, number, boolean)](#getValue-number-number-boolean-)| Gets cell value with given offset from the top-left of this area. |
| [toString()](#toString--)| Returns the reference address of this area. Generally it is the address of the reference which may be used in formula, such as "Sheet1!A1:C3". |
### isExternalLink {#isExternalLink--}
Readonly. Indicates whether this is an external link.
```javascript
isExternalLink : boolean;
```
### externalFileName {#externalFileName--}
Readonly. Get the external file name if this is an external reference.
```javascript
externalFileName : string;
```
### sheetName {#sheetName--}
Readonly. Indicates which sheet this reference is in.
```javascript
sheetName : string;
```
**Remarks**
If it references to multiple worksheets, the returned value is just like the range expression in the formula. For example "Sheet1:Sheet3" for the reference in formula "=SUM(Sheet1:Sheet3!$A$1:$B$2)".
### sheetNames {#sheetNames--}
Readonly. Names of all the worksheets this instance references to.
```javascript
sheetNames : string[];
```
### isEntireRow {#isEntireRow--}
Readonly. Indicates whether this area contains all columns(entire row).
```javascript
isEntireRow : boolean;
```
### isEntireColumn {#isEntireColumn--}
Readonly. Indicates whether this area contains all rows(entire column).
```javascript
isEntireColumn : boolean;
```
### isArea {#isArea--}
Readonly. Indicates whether this is an area.
```javascript
isArea : boolean;
```
**Remarks**
If this is not an area, only StartRow and StartColumn effect.
### endColumn {#endColumn--}
Readonly. The end column of the area.
```javascript
endColumn : number;
```
### startColumn {#startColumn--}
Readonly. The start column of the area.
```javascript
startColumn : number;
```
### endRow {#endRow--}
Readonly. The end row of the area.
```javascript
endRow : number;
```
### startRow {#startRow--}
Readonly. The start row of the area.
```javascript
startRow : number;
```
### getValues() {#getValues--}
Gets cell values in this area.
```javascript
getValues() : VObject;
```
**Returns**
If this area is invalid, "#REF!" will be returned; If this area is one single cell, then return the cell value object; Otherwise return one 2D array for all values in this area.
### getValues(boolean) {#getValues-boolean-}
Gets cell values in this area.
```javascript
getValues(calculateFormulas: boolean) : VObject;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| calculateFormulas | boolean | In this range, if there are some formulas that have not been calculated,         /// this flag denotes whether those formulas should be calculated recursively |
**Returns**
If this area is invalid, "#REF!" will be returned; If this area is one single cell, then return the cell value object; Otherwise return one 2D array for all values in this area.
### getValue(number, number) {#getValue-number-number-}
Gets cell value with given offset from the top-left of this area.
```javascript
getValue(rowOffset: number, colOffset: number) : VObject;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | number | row offset from the start row of this area |
| colOffset | number | column offset from the start row of this area |
**Returns**
"#REF!" if this area is invalid; "#N/A" if given offset out of this area; Otherwise return the cell value at given position.
### getValue(number, number, boolean) {#getValue-number-number-boolean-}
Gets cell value with given offset from the top-left of this area.
```javascript
getValue(rowOffset: number, colOffset: number, calculateFormulas: boolean) : VObject;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | number | row offset from the start row of this area |
| colOffset | number | column offset from the start row of this area |
| calculateFormulas | boolean | Whether calculate it recursively if the specified reference is formula |
**Returns**
"#REF!" if this area is invalid; "#N/A" if given offset out of this area; Otherwise return the cell value at given position.
### toString() {#toString--}
Returns the reference address of this area. Generally it is the address of the reference which may be used in formula, such as "Sheet1!A1:C3".
```javascript
toString() : string;
```
**Returns**
the reference address of this area.
