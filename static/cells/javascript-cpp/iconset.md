##IconSet
Describe the IconSet conditional formatting rule. This conditional formatting rule applies icons to cells according to their values.
## IconSet class
Describe the IconSet conditional formatting rule. This conditional formatting rule applies icons to cells according to their values.
```javascript
class IconSet;
```
### Example
```javascript
const { Workbook, CellArea, FormatConditionType, IconSetType, SaveFormat } = AsposeCells;
//Instantiating a Workbook object
var workbook = new Workbook();
var sheet = workbook.worksheets.get(0);
//Adds an empty conditional formatting
var index = sheet.conditionalFormattings.add();
var fcs = sheet.conditionalFormattings.get(index);
//Sets the conditional format range.
var ca = new CellArea();
ca.startRow = 0;
ca.endRow = 2;
ca.startColumn = 0;
ca.endColumn = 0;
fcs.addArea(ca);
//Adds condition.
var idx = fcs.addCondition(FormatConditionType.IconSet);
fcs.addArea(ca);
var cond = fcs.get(idx);
//Get Icon Set
var iconSet = cond.iconSet;
//Set Icon Type
iconSet.type = IconSetType.Arrows3;
//Put Cell Values
var cell1 = sheet.cells.get("A1");
cell1.putValue(10);
var cell2 = sheet.cells.get("A2");
cell2.putValue(120);
var cell3 = sheet.cells.get("A3");
cell3.putValue(260);
//Saving the Excel file
var uint8Array = workbook.save(SaveFormat.Xlsx);
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [cfIcons](#cfIcons--)| ConditionalFormattingIconCollection | Readonly. Get the[ConditionalFormattingIcon](../conditionalformattingicon/) from the collection |
| [cfvos](#cfvos--)| ConditionalFormattingValueCollection | Readonly. Get the CFValueObjects instance. |
| [type](#type--)| IconSetType | Get or Set the icon set type to display. Setting the type will auto check if the current Cfvos's count is accord with the new type. If not accord, old Cfvos will be cleaned and default Cfvos will be added. |
| [isCustom](#isCustom--)| boolean | Readonly. Indicates whether the icon set is custom. Default value is false. |
| [showValue](#showValue--)| boolean | Get or set the flag indicating whether to show the values of the cells on which this icon set is applied. Default value is true. |
| [reverse](#reverse--)| boolean | Get or set the flag indicating whether to reverses the default order of the icons in this icon set. Default value is false. |
### cfIcons {#cfIcons--}
Readonly. Get the[ConditionalFormattingIcon](../conditionalformattingicon/) from the collection
```javascript
cfIcons : ConditionalFormattingIconCollection;
```
### cfvos {#cfvos--}
Readonly. Get the CFValueObjects instance.
```javascript
cfvos : ConditionalFormattingValueCollection;
```
### type {#type--}
Get or Set the icon set type to display. Setting the type will auto check if the current Cfvos's count is accord with the new type. If not accord, old Cfvos will be cleaned and default Cfvos will be added.
```javascript
type : IconSetType;
```
### isCustom {#isCustom--}
Readonly. Indicates whether the icon set is custom. Default value is false.
```javascript
isCustom : boolean;
```
### showValue {#showValue--}
Get or set the flag indicating whether to show the values of the cells on which this icon set is applied. Default value is true.
```javascript
showValue : boolean;
```
### reverse {#reverse--}
Get or set the flag indicating whether to reverses the default order of the icons in this icon set. Default value is false.
```javascript
reverse : boolean;
```
