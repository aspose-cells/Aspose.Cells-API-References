##CopyOptions
Represents the copy options.
## CopyOptions class
Represents the copy options.
```javascript
class CopyOptions;
```
## Constructors
| Constructor | Description |
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
## Methods
| Method | Description |
| --- | --- |
| [getKeepMacros()](#getKeepMacros--)| <b>@deprecated.</b> Please use the 'keepMacros' property instead. Indicates whether keeping macros; |
| [setKeepMacros(boolean)](#setKeepMacros-boolean-)| <b>@deprecated.</b> Please use the 'keepMacros' property instead. Indicates whether keeping macros; |
| [getExtendToAdjacentRange()](#getExtendToAdjacentRange--)| <b>@deprecated.</b> Please use the 'extendToAdjacentRange' property instead. Indicates whether extend ranges when copying the range to adjacent range. |
| [setExtendToAdjacentRange(boolean)](#setExtendToAdjacentRange-boolean-)| <b>@deprecated.</b> Please use the 'extendToAdjacentRange' property instead. Indicates whether extend ranges when copying the range to adjacent range. |
| [getCopyNames()](#getCopyNames--)| <b>@deprecated.</b> Please use the 'copyNames' property instead. Indicates whether copying the names. |
| [setCopyNames(boolean)](#setCopyNames-boolean-)| <b>@deprecated.</b> Please use the 'copyNames' property instead. Indicates whether copying the names. |
| [getCopyInvalidFormulasAsValues()](#getCopyInvalidFormulasAsValues--)| <b>@deprecated.</b> Please use the 'copyInvalidFormulasAsValues' property instead. If the formula is not valid for the dest destination, only copy values. |
| [setCopyInvalidFormulasAsValues(boolean)](#setCopyInvalidFormulasAsValues-boolean-)| <b>@deprecated.</b> Please use the 'copyInvalidFormulasAsValues' property instead. If the formula is not valid for the dest destination, only copy values. |
| [getColumnCharacterWidth()](#getColumnCharacterWidth--)| <b>@deprecated.</b> Please use the 'columnCharacterWidth' property instead. Indicates whether copying column width in unit of characters. |
| [setColumnCharacterWidth(boolean)](#setColumnCharacterWidth-boolean-)| <b>@deprecated.</b> Please use the 'columnCharacterWidth' property instead. Indicates whether copying column width in unit of characters. |
| [getReferToSheetWithSameName()](#getReferToSheetWithSameName--)| <b>@deprecated.</b> Please use the 'referToSheetWithSameName' property instead. In ms excel, when copying formulas which refer to other worksheets while copying a worksheet to another one, the copied formulas should refer to source workbook. However, for some situations user may need the copied formulas refer to worksheets with the same name in the same workbook, such as when those worksheets have been copied before this copy operation, then this property should be kept as true. |
| [setReferToSheetWithSameName(boolean)](#setReferToSheetWithSameName-boolean-)| <b>@deprecated.</b> Please use the 'referToSheetWithSameName' property instead. In ms excel, when copying formulas which refer to other worksheets while copying a worksheet to another one, the copied formulas should refer to source workbook. However, for some situations user may need the copied formulas refer to worksheets with the same name in the same workbook, such as when those worksheets have been copied before this copy operation, then this property should be kept as true. |
| [getReferToDestinationSheet()](#getReferToDestinationSheet--)| <b>@deprecated.</b> Please use the 'referToDestinationSheet' property instead. When copying the range in the same file and the chart refers to the source sheet, False means the copied chart's data source will not be changed. True means the copied chart's data source refers to the destination sheet. |
| [setReferToDestinationSheet(boolean)](#setReferToDestinationSheet-boolean-)| <b>@deprecated.</b> Please use the 'referToDestinationSheet' property instead. When copying the range in the same file and the chart refers to the source sheet, False means the copied chart's data source will not be changed. True means the copied chart's data source refers to the destination sheet. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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
### getKeepMacros() {#getKeepMacros--}
```javascript
getKeepMacros() : boolean;
```
**Remarks**
Only for copying workbook.
### setKeepMacros(boolean) {#setKeepMacros-boolean-}
```javascript
setKeepMacros(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
Only for copying workbook.
### getExtendToAdjacentRange() {#getExtendToAdjacentRange--}
```javascript
getExtendToAdjacentRange() : boolean;
```
**Remarks**
If it's true, only extends the range of the hyperlink,not adding a new hyperlink when copying hyperlinks to adjacent rows.
### setExtendToAdjacentRange(boolean) {#setExtendToAdjacentRange-boolean-}
```javascript
setExtendToAdjacentRange(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
If it's true, only extends the range of the hyperlink,not adding a new hyperlink when copying hyperlinks to adjacent rows.
### getCopyNames() {#getCopyNames--}
```javascript
getCopyNames() : boolean;
```
### setCopyNames(boolean) {#setCopyNames-boolean-}
```javascript
setCopyNames(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getCopyInvalidFormulasAsValues() {#getCopyInvalidFormulasAsValues--}
```javascript
getCopyInvalidFormulasAsValues() : boolean;
```
### setCopyInvalidFormulasAsValues(boolean) {#setCopyInvalidFormulasAsValues-boolean-}
```javascript
setCopyInvalidFormulasAsValues(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getColumnCharacterWidth() {#getColumnCharacterWidth--}
```javascript
getColumnCharacterWidth() : boolean;
```
### setColumnCharacterWidth(boolean) {#setColumnCharacterWidth-boolean-}
```javascript
setColumnCharacterWidth(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getReferToSheetWithSameName() {#getReferToSheetWithSameName--}
```javascript
getReferToSheetWithSameName() : boolean;
```
**Remarks**
The default value is true.
### setReferToSheetWithSameName(boolean) {#setReferToSheetWithSameName-boolean-}
```javascript
setReferToSheetWithSameName(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
The default value is true.
### getReferToDestinationSheet() {#getReferToDestinationSheet--}
```javascript
getReferToDestinationSheet() : boolean;
```
**Remarks**
The default value is false, it works as MS Excel. For example: if copying a chart with the data source "sheet1!A1:B10" from worksheet "sheet1 to other worksheet "sheet2", The data source will be changed as "sheet2!A1:B10"
### setReferToDestinationSheet(boolean) {#setReferToDestinationSheet-boolean-}
```javascript
setReferToDestinationSheet(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
The default value is false, it works as MS Excel. For example: if copying a chart with the data source "sheet1!A1:B10" from worksheet "sheet1 to other worksheet "sheet2", The data source will be changed as "sheet2!A1:B10"
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
