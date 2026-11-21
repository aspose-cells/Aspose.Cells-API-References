---
title: ConditionalFormattingCollection
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Encapsulates a collection of FormatCondition..formatcondition objects.
type: docs
url: /zh/javascript-cpp/conditionalformattingcollection/
---

## ConditionalFormattingCollection class

Encapsulates a collection of [FormatCondition](../formatcondition/) objects.

```javascript
class ConditionalFormattingCollection;
```


### Example
```javascript
const { Workbook, CellArea, FormatConditionType, OperatorType, Color, SaveFormat } = AsposeCells;

//实例化一个 Workbook 对象
var workbook = new Workbook();
var sheet = workbook.worksheets.get(0);
//获取条件格式
var cformattings = sheet.conditionalFormattings;
//添加空的条件格式
var index = cformattings.add();
//获取新添加的条件格式
var fcs = cformattings.get(index);
//设置条件格式范围。
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
//添加条件。
var conditionIndex = fcs.addCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
//添加条件。
var conditionIndex2 = fcs.addCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");
//设置背景颜色。
var fc = fcs.get(conditionIndex);
fc.style.backgroundColor = Color.Red;
//保存 Excel 文件
var uint8Array = workbook.save(SaveFormat.Xlsx);
```
## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the FormatConditions element at the specified index. |
| [removeArea(number, number, number, number)](#removeArea-number-number-number-number-)| Remove all conditional formatting in the range. |
| [copy(ConditionalFormattingCollection)](#copy-conditionalformattingcollection-)| Copies conditional formatting. |
| [add()](#add--)| Adds a FormatConditions to the collection. |


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


