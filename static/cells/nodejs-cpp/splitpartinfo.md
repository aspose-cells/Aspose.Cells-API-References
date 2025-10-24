##SplitPartInfo
Represents the information of one inputoutput for multiple inputsoutputs such as current page to be rendered when converting spreadsheet to image.
## SplitPartInfo class
Represents the information of one input/output for multiple inputs/outputs, such as current page to be rendered when converting spreadsheet to image.
```javascript
class SplitPartInfo;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [partIndex](#partIndex--)| number | Readonly. Index of current part in sequence(0 based). -1 means there are no multiple parts so the result is single. |
| [sheetIndex](#sheetIndex--)| number | Readonly. Index of the sheet where current part is in. -1 denotes there is only one sheet. |
| [sheetName](#sheetName--)| string | Readonly. Name of the sheet where current part is in. |
## Methods
| Method | Description |
| --- | --- |
| [getPartIndex()](#getPartIndex--)| <b>@deprecated.</b> Please use the 'partIndex' property instead. Index of current part in sequence(0 based). -1 means there are no multiple parts so the result is single. |
| [getSheetIndex()](#getSheetIndex--)| <b>@deprecated.</b> Please use the 'sheetIndex' property instead. Index of the sheet where current part is in. -1 denotes there is only one sheet. |
| [getSheetName()](#getSheetName--)| <b>@deprecated.</b> Please use the 'sheetName' property instead. Name of the sheet where current part is in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### partIndex {#partIndex--}
Readonly. Index of current part in sequence(0 based). -1 means there are no multiple parts so the result is single.
```javascript
partIndex : number;
```
**Remarks**
If multiple sheets need to be processed and every sheet is processed(split) separately, the part index always starts from 0 for every sheet. For example, when converting workbook to images, it represents the output page index of currently processed sheet. And -1 denotes there is only one page for current sheet.
### sheetIndex {#sheetIndex--}
Readonly. Index of the sheet where current part is in. -1 denotes there is only one sheet.
```javascript
sheetIndex : number;
```
### sheetName {#sheetName--}
Readonly. Name of the sheet where current part is in.
```javascript
sheetName : string;
```
**Remarks**
May be null for some situations, such as when rendering the whole workbook to tiff image.
### getPartIndex() {#getPartIndex--}
```javascript
getPartIndex() : number;
```
**Remarks**
If multiple sheets need to be processed and every sheet is processed(split) separately, the part index always starts from 0 for every sheet. For example, when converting workbook to images, it represents the output page index of currently processed sheet. And -1 denotes there is only one page for current sheet.
### getSheetIndex() {#getSheetIndex--}
```javascript
getSheetIndex() : number;
```
### getSheetName() {#getSheetName--}
```javascript
getSheetName() : string;
```
**Remarks**
May be null for some situations, such as when rendering the whole workbook to tiff image.
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
