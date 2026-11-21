---
title: IconSet
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Describe the IconSet conditional formatting rule. This conditional formatting rule applies icons to cells according to their values.
type: docs
url: /ar/javascript-cpp/iconset/
---

## IconSet class

Describe the IconSet conditional formatting rule. This conditional formatting rule applies icons to cells according to their values.

```javascript
class IconSet;
```


### Example
```javascript
const { Workbook, CellArea, FormatConditionType, IconSetType, SaveFormat } = AsposeCells;

//إنشاء كائن Workbook
var workbook = new Workbook();
var sheet = workbook.worksheets.get(0);

//يضيف تنسيقًا شرطيًا فارغًا
var index = sheet.conditionalFormattings.add();
var fcs = sheet.conditionalFormattings.get(index);
//يضبط نطاق التنسيق الشرطي.
var ca = new CellArea();
ca.startRow = 0;
ca.endRow = 2;
ca.startColumn = 0;
ca.endColumn = 0;
fcs.addArea(ca);

//يضيف شرطًا.
var idx = fcs.addCondition(FormatConditionType.IconSet);

fcs.addArea(ca);
var cond = fcs.get(idx);
//احصل على مجموعة الأيقونات
var iconSet = cond.iconSet;
//عيّن نوع الأيقونة
iconSet.type = IconSetType.Arrows3;

//ضع قيم الخلايا
var cell1 = sheet.cells.get("A1");
cell1.putValue(10);
var cell2 = sheet.cells.get("A2");
cell2.putValue(120);
var cell3 = sheet.cells.get("A3");
cell3.putValue(260);

//حفظ ملف Excel
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



