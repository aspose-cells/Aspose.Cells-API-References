---
title: ListColumn
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a column in a Table.
type: docs
url: /nodejs-cpp/listcolumn/
---

## ListColumn class

Represents a column in a Table.

```javascript
class ListColumn;
```


## Methods

| Method | Description |
| --- | --- |
| [getName()](#getName--)| Gets and sets the name of the column. |
| [setName(string)](#setName-string-)| Gets and sets the name of the column. |
| [getTotalsCalculation()](#getTotalsCalculation--)| Gets and sets the type of calculation in the Totals row of the list column. |
| [setTotalsCalculation(TotalsCalculation)](#setTotalsCalculation-totalscalculation-)| Gets and sets the type of calculation in the Totals row of the list column. |
| [getRange()](#getRange--)| Gets the range of this list column. |
| [getFormula()](#getFormula--)| Gets and sets the formula of the list column. |
| [setFormula(string)](#setFormula-string-)| Gets and sets the formula of the list column. |
| [getTotalsRowLabel()](#getTotalsRowLabel--)| Gets and sets the display labels of total row. |
| [setTotalsRowLabel(string)](#setTotalsRowLabel-string-)| Gets and sets the display labels of total row. |
| [getCustomTotalsRowFormula(boolean, boolean)](#getCustomTotalsRowFormula-boolean-boolean-)| Gets the formula of totals row of this list column. |
| [setCustomTotalsRowFormula(string, boolean, boolean)](#setCustomTotalsRowFormula-string-boolean-boolean-)| Gets the formula of totals row of this list column. |
| [getCustomCalculatedFormula(boolean, boolean)](#getCustomCalculatedFormula-boolean-boolean-)| Gets the formula of this list column. |
| [setCustomCalculatedFormula(string, boolean, boolean)](#setCustomCalculatedFormula-string-boolean-boolean-)| Sets the formula for this list column. |
| [getDataStyle()](#getDataStyle--)| Gets the style of the data in this column of the table. |
| [setDataStyle(Style)](#setDataStyle-style-)| Sets the style of the data in this column of the table. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getName() {#getName--}

Gets and sets the name of the column.

```javascript
getName() : string;
```


**Remarks**

If sets the name of the column, the according cell' value will be changed too.

### setName(string) {#setName-string-}

Gets and sets the name of the column.

```javascript
setName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

If sets the name of the column, the according cell' value will be changed too.

### getTotalsCalculation() {#getTotalsCalculation--}

Gets and sets the type of calculation in the Totals row of the list column.

```javascript
getTotalsCalculation() : TotalsCalculation;
```


**Returns**

[TotalsCalculation](../totalscalculation/)

### setTotalsCalculation(TotalsCalculation) {#setTotalsCalculation-totalscalculation-}

Gets and sets the type of calculation in the Totals row of the list column.

```javascript
setTotalsCalculation(value: TotalsCalculation) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TotalsCalculation](../totalscalculation/) | The value to set. |

### getRange() {#getRange--}

Gets the range of this list column.

```javascript
getRange() : Range;
```


**Returns**

[Range](../range/)

### getFormula() {#getFormula--}

Gets and sets the formula of the list column.

```javascript
getFormula() : string;
```


### setFormula(string) {#setFormula-string-}

Gets and sets the formula of the list column.

```javascript
setFormula(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getTotalsRowLabel() {#getTotalsRowLabel--}

Gets and sets the display labels of total row.

```javascript
getTotalsRowLabel() : string;
```


### setTotalsRowLabel(string) {#setTotalsRowLabel-string-}

Gets and sets the display labels of total row.

```javascript
setTotalsRowLabel(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getCustomTotalsRowFormula(boolean, boolean) {#getCustomTotalsRowFormula-boolean-boolean-}

Gets the formula of totals row of this list column.

```javascript
getCustomTotalsRowFormula(isR1C1: boolean, isLocal: boolean) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns**

The formula of this list column.

### setCustomTotalsRowFormula(string, boolean, boolean) {#setCustomTotalsRowFormula-string-boolean-boolean-}

Gets the formula of totals row of this list column.

```javascript
setCustomTotalsRowFormula(formula: string, isR1C1: boolean, isLocal: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | the formula for this list column. |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

### getCustomCalculatedFormula(boolean, boolean) {#getCustomCalculatedFormula-boolean-boolean-}

Gets the formula of this list column.

```javascript
getCustomCalculatedFormula(isR1C1: boolean, isLocal: boolean) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns**

The formula of this list column.

### setCustomCalculatedFormula(string, boolean, boolean) {#setCustomCalculatedFormula-string-boolean-boolean-}

Sets the formula for this list column.

```javascript
setCustomCalculatedFormula(formula: string, isR1C1: boolean, isLocal: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | the formula for this list column. |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

### getDataStyle() {#getDataStyle--}

Gets the style of the data in this column of the table.

```javascript
getDataStyle() : Style;
```


**Returns**

[Style](../style/)

### setDataStyle(Style) {#setDataStyle-style-}

Sets the style of the data in this column of the table.

```javascript
setDataStyle(style: Style) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../style/) |  |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



