---
title: ConditionalFormattingCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates a collection of FormatCondition..formatcondition objects.
type: docs
url: /ar/nodejs-cpp/conditionalformattingcollection/
---

## ConditionalFormattingCollection class

Encapsulates a collection of [FormatCondition](../formatcondition/) objects.

```javascript
class ConditionalFormattingCollection implements Iterable<FormatConditionCollection>;
```


### Example
```javascript
const { Workbook, CellArea, FormatConditionType, OperatorType, Color } = require("aspose.cells.node");

//إنشاء كائن Workbook.
var workbook = new Workbook();
var sheet = workbook.worksheets.get(0);
//الحصول على التنسيقات الشرطية
var cformattings = sheet.conditionalFormattings;
//يضيف تنسيقًا شرطيًا فارغًا
var index = cformattings.add();
//الحصول على التنسيق الشرطي المضاف حديثًا
var fcs = cformattings.get(index);
//يضبط نطاق التنسيق الشرطي.
var ca = new CellArea();
ca.startRow = 0;
ca.endRow = 0;
ca.startColumn = 0;
ca.endColumn = 0;
fcs.addArea(ca);
ca = new CellArea();
ca.startRow = 1;
ca.endRow = 1;
ca.startColumn = 1;
ca.endColumn = 1;
fcs.addArea(ca);
//إضافة شرط.
var conditionIndex = fcs.addCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
//إضافة شرط.
var conditionIndex2 = fcs.addCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");
//يضبط لون الخلفية.
var fc = fcs.get(conditionIndex);
fc.style.backgroundColor = Color.Red;
//حفظ ملف Excel
workbook.save("output/ConditionalFormattingCollection.xls");
```
## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the FormatConditions element at the specified index. |
| [removeArea(number, number, number, number)](#removeArea-number-number-number-number-)| Remove all conditional formatting in the range. |
| [copy(ConditionalFormattingCollection)](#copy-conditionalformattingcollection-)| Copies conditional formatting. |
| [add()](#add--)| Adds a FormatConditions to the collection. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |

## \[Symbol.iterator\](): Iterator\<FormatConditionCollection\>

Returns an iterator over the items in the collection. Enables use of `for...of`, spread syntax, and `Array.from()`.



### get(number) {#get-number-}

Gets the FormatConditions element at the specified index.

```javascript
get(index: number) : FormatConditionCollection;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |

**Returns**

[FormatConditionCollection](../formatconditioncollection/)

### removeArea(number, number, number, number) {#removeArea-number-number-number-number-}

Remove all conditional formatting in the range.

```javascript
removeArea(startRow: number, startColumn: number, totalRows: number, totalColumns: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | number | The start row of the range. |
| startColumn | number | The start column of the range. |
| totalRows | number | The number of rows of the range. |
| totalColumns | number | The number of columns of the range. |

### copy(ConditionalFormattingCollection) {#copy-conditionalformattingcollection-}

Copies conditional formatting.

```javascript
copy(cfs: ConditionalFormattingCollection) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cfs | [ConditionalFormattingCollection](../conditionalformattingcollection/) | The conditional formatting |

### add() {#add--}

Adds a FormatConditions to the collection.

```javascript
add() : number;
```


**Returns**

FormatConditions object index.

### getCount() {#getCount--}

<b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in.

```javascript
getCount() : number;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



