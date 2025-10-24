##CopyOptions
Represents the copy options.
## CopyOptions class
Represents the copy options.
```javascript
class CopyOptions;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| CopyOptions constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [keepMacros](#keepMacros--)| boolean | Indicates whether keeping macros; |
| [extendToAdjacentRange](#extendToAdjacentRange--)| boolean | Indicates whether extend ranges when copying the range to adjacent range. |
| [copyNames](#copyNames--)| boolean | Indicates whether copying the names. |
| [copyInvalidFormulasAsValues](#copyInvalidFormulasAsValues--)| boolean | If the formula is not valid for the dest destination, only copy values. |
| [columnCharacterWidth](#columnCharacterWidth--)| boolean | Indicates whether copying column width in unit of characters. |
| [referToSheetWithSameName](#referToSheetWithSameName--)| boolean | In ms excel, when copying formulas which refer to other worksheets while copying a worksheet to another one, the copied formulas should refer to source workbook. However, for some situations user may need the copied formulas refer to worksheets with the same name in the same workbook, such as when those worksheets have been copied before this copy operation, then this property should be kept as true. |
| [referToDestinationSheet](#referToDestinationSheet--)| boolean | When copying the range in the same file and the chart refers to the source sheet, False means the copied chart's data source will not be changed. True means the copied chart's data source refers to the destination sheet. |
### constructor() {#constructor--}
CopyOptions constructor.
```javascript
constructor();
```
### keepMacros {#keepMacros--}
Indicates whether keeping macros;
```javascript
keepMacros : boolean;
```
**Remarks**
Only for copying workbook.
### extendToAdjacentRange {#extendToAdjacentRange--}
Indicates whether extend ranges when copying the range to adjacent range.
```javascript
extendToAdjacentRange : boolean;
```
**Remarks**
If it's true, only extends the range of the hyperlink,not adding a new hyperlink when copying hyperlinks to adjacent rows.
### copyNames {#copyNames--}
Indicates whether copying the names.
```javascript
copyNames : boolean;
```
### copyInvalidFormulasAsValues {#copyInvalidFormulasAsValues--}
If the formula is not valid for the dest destination, only copy values.
```javascript
copyInvalidFormulasAsValues : boolean;
```
### columnCharacterWidth {#columnCharacterWidth--}
Indicates whether copying column width in unit of characters.
```javascript
columnCharacterWidth : boolean;
```
### referToSheetWithSameName {#referToSheetWithSameName--}
In ms excel, when copying formulas which refer to other worksheets while copying a worksheet to another one, the copied formulas should refer to source workbook. However, for some situations user may need the copied formulas refer to worksheets with the same name in the same workbook, such as when those worksheets have been copied before this copy operation, then this property should be kept as true.
```javascript
referToSheetWithSameName : boolean;
```
**Remarks**
The default value is true.
### referToDestinationSheet {#referToDestinationSheet--}
When copying the range in the same file and the chart refers to the source sheet, False means the copied chart's data source will not be changed. True means the copied chart's data source refers to the destination sheet.
```javascript
referToDestinationSheet : boolean;
```
**Remarks**
The default value is false, it works as MS Excel. For example: if copying a chart with the data source "sheet1!A1:B10" from worksheet "sheet1 to other worksheet "sheet2", The data source will be changed as "sheet2!A1:B10"
