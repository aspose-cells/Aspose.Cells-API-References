##ImportTableOptions
Represents the options of importing data into cells.
## ImportTableOptions class
Represents the options of importing data into cells.
```javascript
class ImportTableOptions;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Creates the default importing options. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [convertGridStyle](#convertGridStyle--)| boolean | Indicates whether apply the style of the grid view to cells. |
| [convertNumericData](#convertNumericData--)| boolean | Gets or sets a value that indicates whether the string value should be converted to numeric or date value. |
| [insertRows](#insertRows--)| boolean | Indicates whether new rows should be added for importing data records. |
| [shiftFirstRowDown](#shiftFirstRowDown--)| boolean | Indicates whether shifting the first row down when inserting rows. |
| [isFieldNameShown](#isFieldNameShown--)| boolean | Indicates whether field name should be imported. |
| [exportCaptionAsFieldName](#exportCaptionAsFieldName--)| boolean | Indicates whether exporting caption as field name |
| [dateFormat](#dateFormat--)| string | Gets or sets date format string for cells with imported datetime values. |
| [numberFormats](#numberFormats--)| string[] | Gets or sets the number formats |
| [isFormulas](#isFormulas--)| boolean[] | Indicates whether the data are formulas. |
| [totalRows](#totalRows--)| number | Gets or sets total row count to import from data source. -1 means all rows of given data source. |
| [totalColumns](#totalColumns--)| number | Gets or sets total column count to import from data source. -1 means all rows of given data source. |
| [columnIndexes](#columnIndexes--)| number[] | Gets or sets the columns(0-based) to import from data source. null means all columns should be imported. |
| [defaultValues](#defaultValues--)| VObject[] | Default value for the value in the table is null. |
| [isHtmlString](#isHtmlString--)| boolean | Indicates whether the value contains html tags. |
| [checkMergedCells](#checkMergedCells--)| boolean | Indicates whether checking merged cells. |
### constructor() {#constructor--}
Creates the default importing options.
```javascript
constructor();
```
### convertGridStyle {#convertGridStyle--}
Indicates whether apply the style of the grid view to cells.
```javascript
convertGridStyle : boolean;
```
### convertNumericData {#convertNumericData--}
Gets or sets a value that indicates whether the string value should be converted to numeric or date value.
```javascript
convertNumericData : boolean;
```
### insertRows {#insertRows--}
Indicates whether new rows should be added for importing data records.
```javascript
insertRows : boolean;
```
### shiftFirstRowDown {#shiftFirstRowDown--}
Indicates whether shifting the first row down when inserting rows.
```javascript
shiftFirstRowDown : boolean;
```
### isFieldNameShown {#isFieldNameShown--}
Indicates whether field name should be imported.
```javascript
isFieldNameShown : boolean;
```
### exportCaptionAsFieldName {#exportCaptionAsFieldName--}
Indicates whether exporting caption as field name
```javascript
exportCaptionAsFieldName : boolean;
```
**Remarks**
Only works for DataTable.
### dateFormat {#dateFormat--}
Gets or sets date format string for cells with imported datetime values.
```javascript
dateFormat : string;
```
### numberFormats {#numberFormats--}
Gets or sets the number formats
```javascript
numberFormats : string[];
```
### isFormulas {#isFormulas--}
Indicates whether the data are formulas.
```javascript
isFormulas : boolean[];
```
### totalRows {#totalRows--}
Gets or sets total row count to import from data source. -1 means all rows of given data source.
```javascript
totalRows : number;
```
### totalColumns {#totalColumns--}
Gets or sets total column count to import from data source. -1 means all rows of given data source.
```javascript
totalColumns : number;
```
### columnIndexes {#columnIndexes--}
Gets or sets the columns(0-based) to import from data source. null means all columns should be imported.
```javascript
columnIndexes : number[];
```
### defaultValues {#defaultValues--}
Default value for the value in the table is null.
```javascript
defaultValues : VObject[];
```
### isHtmlString {#isHtmlString--}
Indicates whether the value contains html tags.
```javascript
isHtmlString : boolean;
```
### checkMergedCells {#checkMergedCells--}
Indicates whether checking merged cells.
```javascript
checkMergedCells : boolean;
```
