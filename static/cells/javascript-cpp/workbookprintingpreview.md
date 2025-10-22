##WorkbookPrintingPreview
Workbook printing preview.
## WorkbookPrintingPreview class
Workbook printing preview.
```javascript
class WorkbookPrintingPreview;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(Workbook, ImageOrPrintOptions)](#constructor-workbook-imageorprintoptions-)| The construct of WorkbookPrintingPreview |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [evaluatedPageCount](#evaluatedPageCount--)| number | Readonly. Evaluate the total page count of this workbook |
### constructor(Workbook, ImageOrPrintOptions) {#constructor-workbook-imageorprintoptions-}
The construct of WorkbookPrintingPreview
```javascript
constructor(workbook: Workbook, options: ImageOrPrintOptions);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| workbook | [Workbook](../workbook/) | Indicate which workbook to be printed. |
| options | [ImageOrPrintOptions](../imageorprintoptions/) | ImageOrPrintOptions contains some property of output |
### evaluatedPageCount {#evaluatedPageCount--}
Readonly. Evaluate the total page count of this workbook
```javascript
evaluatedPageCount : number;
```
