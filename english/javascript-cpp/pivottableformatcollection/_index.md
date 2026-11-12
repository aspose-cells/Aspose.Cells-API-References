---
title: PivotTableFormatCollection
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents the collection of formats applied to PivotTable.
type: docs
url: /javascript-cpp/pivottableformatcollection/
---

## PivotTableFormatCollection class

Represents the collection of formats applied to PivotTable.

```javascript
class PivotTableFormatCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the format by the index. |
| [add()](#add--)| Add a [PivotTableFormat](../pivottableformat/). |
| [format(number, number, Style)](#format-number-number-style-)| Formats the cell in the pivottable area |
| [format(PivotArea, Style)](#format-pivotarea-style-)| Formats selected area of the PivotTable. |
| [format(CellArea, Style)](#format-cellarea-style-)| Formats selected area of the PivotTable. |
| [formatArea(PivotFieldType, number, PivotFieldSubtotalType, PivotTableSelectionType, boolean, boolean, Style)](#formatArea-pivotfieldtype-number-pivotfieldsubtotaltype-pivottableselectiontype-boolean-boolean-style-)| Formats selected area. |


### get(number) {#get-number-}

Gets the format by the index.

```javascript
get(index: number) : PivotTableFormat;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |

**Returns**

[PivotTableFormat](../pivottableformat/)

### add() {#add--}

Add a [PivotTableFormat](../pivottableformat/).

```javascript
add() : number;
```


**Returns**

The index of new format.

### format(number, number, Style) {#format-number-number-style-}

Formats the cell in the pivottable area

```javascript
format(row: number, column: number, style: Style) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Row Index of the cell |
| column | number | Column index of the cell |
| style | [Style](../style/) | Style which is to format the cell |

### format(PivotArea, Style) {#format-pivotarea-style-}

Formats selected area of the PivotTable.

```javascript
format(pivotArea: PivotArea, style: Style) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivotArea | [PivotArea](../pivotarea/) | The selected pivot view area. |
| style | [Style](../style/) | The formatted setting. |

### format(CellArea, Style) {#format-cellarea-style-}

Formats selected area of the PivotTable.

```javascript
format(ca: CellArea, style: Style) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../cellarea/) | The range of the cells. |
| style | [Style](../style/) | The style |

### formatArea(PivotFieldType, number, PivotFieldSubtotalType, PivotTableSelectionType, boolean, boolean, Style) {#formatArea-pivotfieldtype-number-pivotfieldsubtotaltype-pivottableselectiontype-boolean-boolean-style-}

Formats selected area.

```javascript
formatArea(axisType: PivotFieldType, fieldPosition: number, subtotalType: PivotFieldSubtotalType, selectionType: PivotTableSelectionType, isGrandRow: boolean, isGrandColumn: boolean, style: Style) : PivotTableFormat;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| axisType | [PivotFieldType](../pivotfieldtype/) | The region of the PivotTable to which this rule applies. |
| fieldPosition | number | Position of the field within the axis to which this rule applies. |
| subtotalType | [PivotFieldSubtotalType](../pivotfieldsubtotaltype/) | The subtotal filter type of the pivot field |
| selectionType | [PivotTableSelectionType](../pivottableselectiontype/) | Indicates how to select data. |
| isGrandRow | boolean | Indicates whether selecting grand total rows. |
| isGrandColumn | boolean | Indicates whether selecting grand total columns. |
| style | [Style](../style/) | The style which appies to the area of the pivot table. |

**Returns**

[PivotTableFormat](../pivottableformat/)


