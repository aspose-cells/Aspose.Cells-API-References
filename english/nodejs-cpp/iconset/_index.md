---
title: IconSet
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Describe the IconSet conditional formatting rule. This conditional formatting rule applies icons to cells according to their values.
type: docs
url: /nodejs-cpp/iconset/
---

## IconSet class

Describe the IconSet conditional formatting rule. This conditional formatting rule applies icons to cells according to their values.

```javascript
class IconSet;
```


### Example
```javascript
const { Workbook, CellArea, FormatConditionType, IconSetType } = require("aspose.cells.node");

//Instantiating a Workbook object
var workbook = new Workbook();
var sheet = workbook.getWorksheets().get(0);

//Adds an empty conditional formatting
var index = sheet.getConditionalFormattings().add();
var fcs = sheet.getConditionalFormattings().get(index);
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
var iconSet = cond.getIconSet();
//Set Icon Type
iconSet.setType(IconSetType.Arrows3);

//Put Cell Values
var cell1 = sheet.getCells().get("A1");
cell1.putValue(10);
var cell2 = sheet.getCells().get("A2");
cell2.putValue(120);
var cell3 = sheet.getCells().get("A3");
cell3.putValue(260);

//Saving the Excel file
workbook.save("output/IconSet.xlsx");
```
## Methods

| Method | Description |
| --- | --- |
| [getCfIcons()](#getCfIcons--)| Get the[ConditionalFormattingIcon](../conditionalformattingicon/) from the collection |
| [getCfvos()](#getCfvos--)| Get the CFValueObjects instance. |
| [getType()](#getType--)| Get or Set the icon set type to display. Setting the type will auto check if the current Cfvos's count is accord with the new type. If not accord, old Cfvos will be cleaned and default Cfvos will be added. |
| [setType(IconSetType)](#setType-iconsettype-)| Get or Set the icon set type to display. Setting the type will auto check if the current Cfvos's count is accord with the new type. If not accord, old Cfvos will be cleaned and default Cfvos will be added. |
| [isCustom()](#isCustom--)| Indicates whether the icon set is custom. Default value is false. |
| [getShowValue()](#getShowValue--)| Get or set the flag indicating whether to show the values of the cells on which this icon set is applied. Default value is true. |
| [setShowValue(boolean)](#setShowValue-boolean-)| Get or set the flag indicating whether to show the values of the cells on which this icon set is applied. Default value is true. |
| [getReverse()](#getReverse--)| Get or set the flag indicating whether to reverses the default order of the icons in this icon set. Default value is false. |
| [setReverse(boolean)](#setReverse-boolean-)| Get or set the flag indicating whether to reverses the default order of the icons in this icon set. Default value is false. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getCfIcons() {#getCfIcons--}

Get the[ConditionalFormattingIcon](../conditionalformattingicon/) from the collection

```javascript
getCfIcons() : ConditionalFormattingIconCollection;
```


**Returns**

[ConditionalFormattingIconCollection](../conditionalformattingiconcollection/)

### getCfvos() {#getCfvos--}

Get the CFValueObjects instance.

```javascript
getCfvos() : ConditionalFormattingValueCollection;
```


**Returns**

[ConditionalFormattingValueCollection](../conditionalformattingvaluecollection/)

### getType() {#getType--}

Get or Set the icon set type to display. Setting the type will auto check if the current Cfvos's count is accord with the new type. If not accord, old Cfvos will be cleaned and default Cfvos will be added.

```javascript
getType() : IconSetType;
```


**Returns**

[IconSetType](../iconsettype/)

### setType(IconSetType) {#setType-iconsettype-}

Get or Set the icon set type to display. Setting the type will auto check if the current Cfvos's count is accord with the new type. If not accord, old Cfvos will be cleaned and default Cfvos will be added.

```javascript
setType(value: IconSetType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IconSetType](../iconsettype/) | The value to set. |

### isCustom() {#isCustom--}

Indicates whether the icon set is custom. Default value is false.

```javascript
isCustom() : boolean;
```


### getShowValue() {#getShowValue--}

Get or set the flag indicating whether to show the values of the cells on which this icon set is applied. Default value is true.

```javascript
getShowValue() : boolean;
```


### setShowValue(boolean) {#setShowValue-boolean-}

Get or set the flag indicating whether to show the values of the cells on which this icon set is applied. Default value is true.

```javascript
setShowValue(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getReverse() {#getReverse--}

Get or set the flag indicating whether to reverses the default order of the icons in this icon set. Default value is false.

```javascript
getReverse() : boolean;
```


### setReverse(boolean) {#setReverse-boolean-}

Get or set the flag indicating whether to reverses the default order of the icons in this icon set. Default value is false.

```javascript
setReverse(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



