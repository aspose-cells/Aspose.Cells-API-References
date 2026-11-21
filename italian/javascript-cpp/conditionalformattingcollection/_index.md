---
title: ConditionalFormattingCollection
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Encapsulates a collection of FormatCondition..formatcondition objects.
type: docs
url: /it/javascript-cpp/conditionalformattingcollection/
---

## ConditionalFormattingCollection class

Encapsulates a collection of [FormatCondition](../formatcondition/) objects.

```javascript
class ConditionalFormattingCollection;
```


### Example
```javascript
const { Workbook, CellArea, FormatConditionType, OperatorType, Color, SaveFormat } = AsposeCells;

//Istanziare un oggetto Workbook
var workbook = new Workbook();
var sheet = workbook.worksheets.get(0);
//Ottieni formattazioni condizionali
var cformattings = sheet.conditionalFormattings;
//Aggiunge una formattazione condizionale vuota
var index = cformattings.add();
//Ottieni la formattazione condizionale appena aggiunta
var fcs = cformattings.get(index);
//Imposta l'intervallo di formattazione condizionale.
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
//Aggiungi condizione.
var conditionIndex = fcs.addCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
//Aggiungi condizione.
var conditionIndex2 = fcs.addCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");
//Imposta il colore di sfondo.
var fc = fcs.get(conditionIndex);
fc.style.backgroundColor = Color.Red;
//Salvare il file Excel
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


