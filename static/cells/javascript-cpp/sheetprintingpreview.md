##SheetPrintingPreview
Worksheet printing preview.
## SheetPrintingPreview class
Worksheet printing preview.
```javascript
class SheetPrintingPreview;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(Worksheet, ImageOrPrintOptions)](#constructor-worksheet-imageorprintoptions-)| The construct of SheetPrintingPreview |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [evaluatedPageCount](#evaluatedPageCount--)| number | Readonly. Evaluate the total page count of this worksheet |
### constructor(Worksheet, ImageOrPrintOptions) {#constructor-worksheet-imageorprintoptions-}
The construct of SheetPrintingPreview
```javascript
constructor(sheet: Worksheet, options: ImageOrPrintOptions);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheet | [Worksheet](../worksheet/) | Indicate which spreadsheet to be printed. |
| options | [ImageOrPrintOptions](../imageorprintoptions/) | ImageOrPrintOptions contains some property of output |
### evaluatedPageCount {#evaluatedPageCount--}
Readonly. Evaluate the total page count of this worksheet
```javascript
evaluatedPageCount : number;
```
