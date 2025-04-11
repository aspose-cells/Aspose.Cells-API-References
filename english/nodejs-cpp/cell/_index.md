﻿---
title: Cell
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates the object that represents a single Workbook cell.
type: docs
url: /nodejs-cpp/cell/
---

## Cell class

Encapsulates the object that represents a single Workbook cell.

```javascript
class Cell;
```


### Example
```javascript
const { Workbook, Color, TextAlignmentType } = require("aspose.cells.node");

var excel = new Workbook();
var cells = excel.getWorksheets().get(0).getCells();

//Put a string into a cell
var cell = cells.get(0, 0);
cell.putValue("Hello");
var first = cell.getStringValue();
//Put an integer into a cell
cell = cells.get("B1");
cell.putValue(12);
var second = cell.getIntValue();
//Put a double into a cell
cell = cells.get(0, 2);
cell.putValue(-1.234);
var third = cell.getDoubleValue();
//Put a formula into a cell
cell = cells.get("D1");
cell.setFormula("=B1 + C1");
//Put a combined formula: "sum(average(b1,c1), b1)" to cell at b2
cell = cells.get("b2");
cell.setFormula("=sum(average(b1,c1), b1)");

//Set style of a cell
var style = cell.getStyle();
//Set background color
style.setBackgroundColor(Color.Yellow);
//Set format of a cell
style.getFont().setName("Courier New");
style.setVerticalAlignment(TextAlignmentType.Top);
cell.setStyle(style);
```
## Methods

| Method | Description |
| --- | --- |
| [getWorksheet()](#getWorksheet--)| Gets the parent worksheet. |
| [getDateTimeValue()](#getDateTimeValue--)| Gets the DateTime value contained in the cell. |
| [getRow()](#getRow--)| Gets row number (zero based) of the cell. |
| [getColumn()](#getColumn--)| Gets column number (zero based) of the cell. |
| [isFormula()](#isFormula--)| Represents if the specified cell contains formula. |
| [getHasCustomFunction()](#getHasCustomFunction--)| Checks whether there is custom function(unsupported function) in this cell's formula. |
| [getType()](#getType--)| Represents cell value type. |
| [getName()](#getName--)| Gets the name of the cell. |
| [isErrorValue()](#isErrorValue--)| Checks if the value of this cell is an error. |
| [isNumericValue()](#isNumericValue--)| Indicates whether the value of this cell is numeric(int, double and datetime) |
| [getStringValue()](#getStringValue--)| Gets the string value contained in the cell. If the type of this cell is string, then return the string value itself. For other cell types, the formatted string value (formatted with the specified style of this cell) will be returned. The formatted cell value is same with what you can get from excel when copying a cell as text(such as copying cell to text editor or exporting to csv). |
| [getNumberCategoryType()](#getNumberCategoryType--)| Represents the category type of this cell's number formatting. |
| [getDisplayStringValue()](#getDisplayStringValue--)| Gets the formatted string value of this cell by cell's display style. |
| [getIntValue()](#getIntValue--)| Gets the integer value contained in the cell. |
| [getDoubleValue()](#getDoubleValue--)| Gets the double value contained in the cell. |
| [getFloatValue()](#getFloatValue--)| Gets the float value contained in the cell. |
| [getBoolValue()](#getBoolValue--)| Gets the boolean value contained in the cell. |
| [getHasCustomStyle()](#getHasCustomStyle--)| Indicates whether this cell has custom style settings(different from the default one inherited from corresponding row, column, or workbook). |
| [getSharedStyleIndex()](#getSharedStyleIndex--)| Gets cell's shared style index in the style pool. |
| [getFormula()](#getFormula--)| Gets or sets a formula of the [Cell](../cell/). |
| [setFormula(string)](#setFormula-string-)| Gets or sets a formula of the [Cell](../cell/). |
| [getFormulaLocal()](#getFormulaLocal--)| Get the locale formatted formula of the cell. |
| [setFormulaLocal(string)](#setFormulaLocal-string-)| Get the locale formatted formula of the cell. |
| [getR1C1Formula()](#getR1C1Formula--)| Gets or sets a R1C1 formula of the [Cell](../cell/). |
| [setR1C1Formula(string)](#setR1C1Formula-string-)| Gets or sets a R1C1 formula of the [Cell](../cell/). |
| [getContainsExternalLink()](#getContainsExternalLink--)| Indicates whether this cell contains an external link. Only applies when the cell is a formula cell. |
| [isArrayHeader()](#isArrayHeader--)| Indicates the cell's formula is an array formula and it is the first cell of the array. |
| [isDynamicArrayFormula()](#isDynamicArrayFormula--)| Indicates whether the cell's formula is dynamic array formula(true) or legacy array formula(false). |
| [isArrayFormula()](#isArrayFormula--)| Indicates whether the cell formula is an array formula. |
| [isSharedFormula()](#isSharedFormula--)| Indicates whether the cell formula is part of shared formula. |
| [isTableFormula()](#isTableFormula--)| Indicates whether this cell is part of table formula. |
| [getValue()](#getValue--)| Gets/sets the value contained in this cell. |
| [setValue(Object)](#setValue-object-)| Gets/sets the value contained in this cell. |
| [isStyleSet()](#isStyleSet--)| Indicates if the cell's style is set. If return false, it means this cell has a default cell format. |
| [isMerged()](#isMerged--)| Checks if a cell is part of a merged range or not. |
| [getComment()](#getComment--)| Gets the comment of this cell. |
| [getHtmlString()](#getHtmlString--)| Gets and sets the html string which contains data and some formats in this cell. |
| [setHtmlString(string)](#setHtmlString-string-)| Gets and sets the html string which contains data and some formats in this cell. |
| [isCheckBoxStyle()](#isCheckBoxStyle--)| Indicates whether setting this cell as a check box. |
| [setIsCheckBoxStyle(boolean)](#setIsCheckBoxStyle-boolean-)| Indicates whether setting this cell as a check box. |
| [getEmbeddedImage()](#getEmbeddedImage--)| Gets and sets the embeddedn image in the cell. |
| [setEmbeddedImage(Uint8Array)](#setEmbeddedImage-uint8array-)| Gets and sets the embeddedn image in the cell. |
| [calculate(CalculationOptions)](#calculate-calculationoptions-)| Calculates the formula of the cell. |
| [putValue(boolean)](#putValue-boolean-)| Puts a boolean value into the cell. |
| [putValue(number)](#putValue-number-)| Puts an integer value into the cell. |
| [putValue(number)](#putValue-number-)| Puts a double value into the cell. |
| [putValue(string, boolean, boolean)](#putValue-string-boolean-boolean-)| Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will be reset. |
| [putValue(string, boolean)](#putValue-string-boolean-)| Puts a string value into the cell and converts the value to other data type if appropriate. |
| [putValue(string)](#putValue-string-)| Puts a string value into the cell. |
| [putValue(Date)](#putValue-date-)| Puts a DateTime value into the cell. |
| [putValue(Object)](#putValue-object-)| Puts an object value into the cell. |
| [getStringValue(CellValueFormatStrategy)](#getStringValue-cellvalueformatstrategy-)| Gets the string value by specific formatted strategy. |
| [getWidthOfValue()](#getWidthOfValue--)| Gets the width of the value in unit of pixels. |
| [getHeightOfValue()](#getHeightOfValue--)| Gets the height of the value in unit of pixels. |
| [getDisplayStyle()](#getDisplayStyle--)| Gets the display style of this cell. |
| [getDisplayStyle(boolean)](#getDisplayStyle-boolean-)| Gets the display style of this cell. |
| [getDisplayStyle(BorderType)](#getDisplayStyle-bordertype-)| Gets the display style of this cell. |
| [getFormatConditions()](#getFormatConditions--)| Gets format conditions which applies to this cell. |
| [getStyle()](#getStyle--)| Gets the cell style. |
| [getStyle(boolean)](#getStyle-boolean-)| If checkBorders is true, check whether other cells' borders will effect the style of this cell. |
| [setStyle(Style)](#setStyle-style-)| Sets the cell style. |
| [setStyle(Style, boolean)](#setStyle-style-boolean-)| Apply the changed property of style to the cell. |
| [setStyle(Style, StyleFlag)](#setStyle-style-styleflag-)| Apply the cell style based on flags. |
| [setFormula(string, Object)](#setFormula-string-object-)| Set the formula and the value(calculated result) of the formula. |
| [setFormula(string, FormulaParseOptions)](#setFormula-string-formulaparseoptions-)| Set the formula and the value(calculated result) of the formula. |
| [setFormula(string, FormulaParseOptions, Object)](#setFormula-string-formulaparseoptions-object-)| Set the formula and the value(calculated result) of the formula. |
| [getFormula(boolean, boolean)](#getFormula-boolean-boolean-)| Get the formula of this cell. |
| [setArrayFormula(string, number, number)](#setArrayFormula-string-number-number-)| Sets an array formula(legacy array formula entered via CTRL+SHIFT+ENTER in ms excel) to a range of cells. |
| [setArrayFormula(string, number, number, FormulaParseOptions)](#setArrayFormula-string-number-number-formulaparseoptions-)| Sets an array formula to a range of cells. |
| [setArrayFormula(string, number, number, FormulaParseOptions, Object[][])](#setArrayFormula-string-number-number-formulaparseoptions-objectarrayarray-)| Sets an array formula to a range of cells. |
| [setSharedFormula(string, number, number)](#setSharedFormula-string-number-number-)| Sets shared formulas to a range of cells. |
| [setSharedFormula(string, number, number, FormulaParseOptions)](#setSharedFormula-string-number-number-formulaparseoptions-)| Sets shared formulas to a range of cells. |
| [setSharedFormula(string, number, number, FormulaParseOptions, Object[][])](#setSharedFormula-string-number-number-formulaparseoptions-objectarrayarray-)| Sets shared formulas to a range of cells. |
| [getPrecedents()](#getPrecedents--)| Gets all references appearing in this cell's formula. |
| [getDependents(boolean)](#getDependents-boolean-)| Get all cells whose formula references to this cell directly. |
| [getPrecedentsInCalculation()](#getPrecedentsInCalculation--)| Gets all precedents(reference to cells in current workbook) used by this cell's formula while calculating it. |
| [getDependentsInCalculation(boolean)](#getDependentsInCalculation-boolean-)| Gets all cells whose calculated result depends on this cell. |
| [getArrayRange()](#getArrayRange--)| Gets the array range if the cell's formula is an array formula. |
| [setDynamicArrayFormula(string, FormulaParseOptions, boolean)](#setDynamicArrayFormula-string-formulaparseoptions-boolean-)| Sets dynamic array formula and make the formula spill into neighboring cells if possible. |
| [setDynamicArrayFormula(string, FormulaParseOptions, Object[][], boolean, boolean)](#setDynamicArrayFormula-string-formulaparseoptions-objectarrayarray-boolean-boolean-)| Sets dynamic array formula and make the formula spill into neighboring cells if possible. |
| [setDynamicArrayFormula(string, FormulaParseOptions, Object[][], boolean, boolean, CalculationOptions)](#setDynamicArrayFormula-string-formulaparseoptions-objectarrayarray-boolean-boolean-calculationoptions-)| Sets dynamic array formula and make the formula spill into neighboring cells if possible. |
| [setTableFormula(number, number, string, string, Object[][])](#setTableFormula-number-number-string-string-objectarrayarray-)| Create two-variable data table for given range starting from this cell. |
| [setTableFormula(number, number, string, boolean, Object[][])](#setTableFormula-number-number-string-boolean-objectarrayarray-)| Create one-variable data table for given range starting from this cell. |
| [setTableFormula(number, number, number, number, number, number, Object[][])](#setTableFormula-number-number-number-number-number-number-objectarrayarray-)| Create two-variable data table for given range starting from this cell. |
| [setTableFormula(number, number, number, number, boolean, Object[][])](#setTableFormula-number-number-number-number-boolean-objectarrayarray-)| Create one-variable data table for given range starting from this cell. |
| [removeArrayFormula(boolean)](#removeArrayFormula-boolean-)| Remove array formula. |
| [copy(Cell)](#copy-cell-)| Copies data from a source cell. |
| [characters(number, number)](#characters-number-number-)| Returns a Characters object that represents a range of characters within the cell text. |
| [replace(string, string, ReplaceOptions)](#replace-string-string-replaceoptions-)| Replace text of the cell with options. |
| [insertText(number, string)](#insertText-number-string-)| Insert some characters to the cell. If the cell is rich formatted, this method could keep the original formatting. |
| [isRichText()](#isRichText--)| Indicates whether the string value of this cell is a rich formatted text. |
| [getCharacters()](#getCharacters--)| Returns all Characters objects that represents a range of characters within the cell text. |
| [getCharacters(boolean)](#getCharacters-boolean-)| Returns all Characters objects that represents a range of characters within the cell text. |
| [setCharacters(FontSetting[])](#setCharacters-fontsettingarray-)| Sets rich text format of the cell. |
| [getMergedRange()](#getMergedRange--)| Returns a [Range](../range/) object which represents a merged range. |
| [getHtmlString(boolean)](#getHtmlString-boolean-)| Gets the html string which contains data and some formats in this cell. |
| [toString()](#toString--)| Returns a string represents the current Cell object. |
| [toJson()](#toJson--)| Convert [Cell](../cell/) to JSON struct data. |
| [equals(Object)](#equals-object-)| Checks whether this object refers to the same cell with another. |
| [equals(Cell)](#equals-cell-)| Checks whether this object refers to the same cell with another cell object. |
| [getHashCode()](#getHashCode--)| Serves as a hash function for a particular type. |
| [getConditionalFormattingResult()](#getConditionalFormattingResult--)| Get the result of the conditional formatting. |
| [getValidation()](#getValidation--)| Gets the validation applied to this cell. |
| [getValidationValue()](#getValidationValue--)| Gets the value of validation which applied to this cell. |
| [getTable()](#getTable--)| Gets the table which contains this cell. |
| [getRichValue()](#getRichValue--)| Gets rich value of the cell. |
| [dispose()](#dispose--)|  |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getWorksheet() {#getWorksheet--}

Gets the parent worksheet.

```javascript
getWorksheet() : Worksheet;
```


**Returns**

[Worksheet](../worksheet/)

### getDateTimeValue() {#getDateTimeValue--}

Gets the DateTime value contained in the cell.

```javascript
getDateTimeValue() : Date;
```


### getRow() {#getRow--}

Gets row number (zero based) of the cell.

```javascript
getRow() : number;
```


### getColumn() {#getColumn--}

Gets column number (zero based) of the cell.

```javascript
getColumn() : number;
```


### isFormula() {#isFormula--}

Represents if the specified cell contains formula.

```javascript
isFormula() : boolean;
```


### getHasCustomFunction() {#getHasCustomFunction--}

Checks whether there is custom function(unsupported function) in this cell's formula.

```javascript
getHasCustomFunction() : boolean;
```


### getType() {#getType--}

Represents cell value type.

```javascript
getType() : CellValueType;
```


**Returns**

[CellValueType](../cellvaluetype/)

### getName() {#getName--}

Gets the name of the cell.

```javascript
getName() : string;
```


**Remarks**

A cell name includes its column letter and row number. For example, the name of a cell in row 0 and column 0 is A1.

### isErrorValue() {#isErrorValue--}

Checks if the value of this cell is an error.

```javascript
isErrorValue() : boolean;
```


**Remarks**

Also applies to formula cell to check whether the calculated result is an error.

### isNumericValue() {#isNumericValue--}

Indicates whether the value of this cell is numeric(int, double and datetime)

```javascript
isNumericValue() : boolean;
```


**Remarks**

Also applies to formula cell to check the calculated result

### getStringValue() {#getStringValue--}

Gets the string value contained in the cell. If the type of this cell is string, then return the string value itself. For other cell types, the formatted string value (formatted with the specified style of this cell) will be returned. The formatted cell value is same with what you can get from excel when copying a cell as text(such as copying cell to text editor or exporting to csv).

```javascript
getStringValue() : string;
```


### getNumberCategoryType() {#getNumberCategoryType--}

Represents the category type of this cell's number formatting.

```javascript
getNumberCategoryType() : NumberCategoryType;
```


**Returns**

[NumberCategoryType](../numbercategorytype/)

**Remarks**

When cell's formatting pattern is combined with conditional formatting patterns, then the returned type is corresponding to the part which is used for current value of this cell. For example, if the formatting pattern for this cell is "#,##0;(#,##0);"-";@", then when cell's value is numeric and not 0, the returned type is [NumberCategoryType.Number](../numbercategorytype.number/); When cell's value is 0 or not numeric value, the returned type is [NumberCategoryType.Text](../numbercategorytype.text/).

### getDisplayStringValue() {#getDisplayStringValue--}

Gets the formatted string value of this cell by cell's display style.

```javascript
getDisplayStringValue() : string;
```


### getIntValue() {#getIntValue--}

Gets the integer value contained in the cell.

```javascript
getIntValue() : number;
```


### getDoubleValue() {#getDoubleValue--}

Gets the double value contained in the cell.

```javascript
getDoubleValue() : number;
```


### getFloatValue() {#getFloatValue--}

Gets the float value contained in the cell.

```javascript
getFloatValue() : number;
```


### getBoolValue() {#getBoolValue--}

Gets the boolean value contained in the cell.

```javascript
getBoolValue() : boolean;
```


### getHasCustomStyle() {#getHasCustomStyle--}

Indicates whether this cell has custom style settings(different from the default one inherited from corresponding row, column, or workbook).

```javascript
getHasCustomStyle() : boolean;
```


### getSharedStyleIndex() {#getSharedStyleIndex--}

Gets cell's shared style index in the style pool.

```javascript
getSharedStyleIndex() : number;
```


### getFormula() {#getFormula--}

Gets or sets a formula of the [Cell](../cell/).

```javascript
getFormula() : string;
```


**Remarks**

A formula string always begins with an equal sign (=). And please always use comma(,) as parameters delimiter, such as "=SUM(A1, E1, H2)".

### setFormula(string) {#setFormula-string-}

Gets or sets a formula of the [Cell](../cell/).

```javascript
setFormula(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

A formula string always begins with an equal sign (=). And please always use comma(,) as parameters delimiter, such as "=SUM(A1, E1, H2)".

**Example**
```javascript
const { Workbook } = require("aspose.cells.node");

var excel = new Workbook();
var cells = excel.getWorksheets().get(0).getCells();
cells.get("B6").setFormula("=SUM(B2:B5, E1) + sheet2!A1");
```

### getFormulaLocal() {#getFormulaLocal--}

Get the locale formatted formula of the cell.

```javascript
getFormulaLocal() : string;
```


### setFormulaLocal(string) {#setFormulaLocal-string-}

Get the locale formatted formula of the cell.

```javascript
setFormulaLocal(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getR1C1Formula() {#getR1C1Formula--}

Gets or sets a R1C1 formula of the [Cell](../cell/).

```javascript
getR1C1Formula() : string;
```


### setR1C1Formula(string) {#setR1C1Formula-string-}

Gets or sets a R1C1 formula of the [Cell](../cell/).

```javascript
setR1C1Formula(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getContainsExternalLink() {#getContainsExternalLink--}

Indicates whether this cell contains an external link. Only applies when the cell is a formula cell.

```javascript
getContainsExternalLink() : boolean;
```


### isArrayHeader() {#isArrayHeader--}

Indicates the cell's formula is an array formula and it is the first cell of the array.

```javascript
isArrayHeader() : boolean;
```


### isDynamicArrayFormula() {#isDynamicArrayFormula--}

Indicates whether the cell's formula is dynamic array formula(true) or legacy array formula(false).

```javascript
isDynamicArrayFormula() : boolean;
```


### isArrayFormula() {#isArrayFormula--}

Indicates whether the cell formula is an array formula.

```javascript
isArrayFormula() : boolean;
```


### isSharedFormula() {#isSharedFormula--}

Indicates whether the cell formula is part of shared formula.

```javascript
isSharedFormula() : boolean;
```


### isTableFormula() {#isTableFormula--}

Indicates whether this cell is part of table formula.

```javascript
isTableFormula() : boolean;
```


### getValue() {#getValue--}

Gets/sets the value contained in this cell.

```javascript
getValue() : Object;
```


**Remarks**

Possible type: <p>null,</p> <p>Boolean,</p> <p>DateTime,</p> <p>Double,</p> <p>Integer</p> <p>String.</p> For int value, it may be returned as an Integer object or a Double object. And there is no guarantee that the returned value will be kept as the same type of object always.

### setValue(Object) {#setValue-object-}

Gets/sets the value contained in this cell.

```javascript
setValue(value: Object) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Object | The value to set. |

**Remarks**

Possible type: <p>null,</p> <p>Boolean,</p> <p>DateTime,</p> <p>Double,</p> <p>Integer</p> <p>String.</p> For int value, it may be returned as an Integer object or a Double object. And there is no guarantee that the returned value will be kept as the same type of object always.

### isStyleSet() {#isStyleSet--}

Indicates if the cell's style is set. If return false, it means this cell has a default cell format.

```javascript
isStyleSet() : boolean;
```


### isMerged() {#isMerged--}

Checks if a cell is part of a merged range or not.

```javascript
isMerged() : boolean;
```


### getComment() {#getComment--}

Gets the comment of this cell.

```javascript
getComment() : Comment;
```


**Returns**

[Comment](../comment/)

**Remarks**

If there is no comment applies to the cell, returns null.

### getHtmlString() {#getHtmlString--}

Gets and sets the html string which contains data and some formats in this cell.

```javascript
getHtmlString() : string;
```


### setHtmlString(string) {#setHtmlString-string-}

Gets and sets the html string which contains data and some formats in this cell.

```javascript
setHtmlString(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isCheckBoxStyle() {#isCheckBoxStyle--}

Indicates whether setting this cell as a check box.

```javascript
isCheckBoxStyle() : boolean;
```


### setIsCheckBoxStyle(boolean) {#setIsCheckBoxStyle-boolean-}

Indicates whether setting this cell as a check box.

```javascript
setIsCheckBoxStyle(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getEmbeddedImage() {#getEmbeddedImage--}

Gets and sets the embeddedn image in the cell.

```javascript
getEmbeddedImage() : Uint8Array;
```


### setEmbeddedImage(Uint8Array) {#setEmbeddedImage-uint8array-}

Gets and sets the embeddedn image in the cell.

```javascript
setEmbeddedImage(value: Uint8Array) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number[] | The value to set. |

### calculate(CalculationOptions) {#calculate-calculationoptions-}

Calculates the formula of the cell.

```javascript
calculate(options: CalculationOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [CalculationOptions](../calculationoptions/) | Options for calculation |

### putValue(boolean) {#putValue-boolean-}

Puts a boolean value into the cell.

```javascript
putValue(boolValue: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| boolValue | boolean |  |

### putValue(number) {#putValue-number-}

Puts an integer value into the cell.

```javascript
putValue(intValue: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| intValue | number | Input value |

### putValue(number) {#putValue-number-}

Puts a double value into the cell.

```javascript
putValue(doubleValue: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| doubleValue | number | Input value |

### putValue(string, boolean, boolean) {#putValue-string-boolean-boolean-}

Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will be reset.

```javascript
putValue(stringValue: string, isConverted: boolean, setStyle: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | string | Input value |
| isConverted | boolean | True: converted to other data type if appropriate. |
| setStyle | boolean | True: set the number format to cell's style when converting to other data type |

### putValue(string, boolean) {#putValue-string-boolean-}

Puts a string value into the cell and converts the value to other data type if appropriate.

```javascript
putValue(stringValue: string, isConverted: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | string | Input value |
| isConverted | boolean | True: converted to other data type if appropriate. |

### putValue(string) {#putValue-string-}

Puts a string value into the cell.

```javascript
putValue(stringValue: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | string | Input value |

### putValue(Date) {#putValue-date-}

Puts a DateTime value into the cell.

```javascript
putValue(dateTime: Date) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dateTime | Date | Input value |

**Remarks**

Setting a DateTime value for a cell dose not means the cell will be formatted as date time automatically. DateTime value was maintained as numeric value in the data model of both ms excel and Aspose.Cells. Whether the numeric value will be taken as the numeric value itself or date time depends on the number format applied on this cell. If this cell has not been formatted as date time, it will be displayed as a numeric value even though what you input is DateTime.

### putValue(Object) {#putValue-object-}

Puts an object value into the cell.

```javascript
putValue(objectValue: Object) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| objectValue | Object | input value |

### getStringValue(CellValueFormatStrategy) {#getStringValue-cellvalueformatstrategy-}

Gets the string value by specific formatted strategy.

```javascript
getStringValue(formatStrategy: CellValueFormatStrategy) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formatStrategy | [CellValueFormatStrategy](../cellvalueformatstrategy/) | The formatted strategy. |

### getWidthOfValue() {#getWidthOfValue--}

Gets the width of the value in unit of pixels.

```javascript
getWidthOfValue() : number;
```


### getHeightOfValue() {#getHeightOfValue--}

Gets the height of the value in unit of pixels.

```javascript
getHeightOfValue() : number;
```


### getDisplayStyle() {#getDisplayStyle--}

Gets the display style of this cell.

```javascript
getDisplayStyle() : Style;
```


**Returns**

display style of this cell

**Remarks**

Same with using [BorderType.SideBorders](../bordertype.sideborders/) for [GetDisplayStyle(BorderType)](../getdisplaystyle(bordertype)/). That is, this method will check and adjust top/bottom/left/right borders of this cell according to the style([GetStyle()](../getstyle()/)) of its adjacent cells, but do not check the merged cells, and do not check the display style of adjacent cells.

### getDisplayStyle(boolean) {#getDisplayStyle-boolean-}

Gets the display style of this cell.

```javascript
getDisplayStyle(includeMergedBorders: boolean) : Style;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| includeMergedBorders | boolean | Indicates whether checking borders of merged cells. |

**Returns**

display style of this cell

**Remarks**

If the specified flag is false, then it is same with [GetDisplayStyle()](../getdisplaystyle()/). Otherwise it is same with using [BorderType.SideBorders](../bordertype.sideborders/)|[BorderType.DynamicStyleBorders](../bordertype.dynamicstyleborders/) for [GetDisplayStyle(BorderType)](../getdisplaystyle(bordertype)/).

### getDisplayStyle(BorderType) {#getDisplayStyle-bordertype-}

Gets the display style of this cell.

```javascript
getDisplayStyle(adjacentBorders: BorderType) : Style;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| adjacentBorders | [BorderType](../bordertype/) | Indicates which borders need to be checked and adjusted         /// according to the borders of adjacent cells. |

**Returns**

display style of this cell

**Remarks**

If this cell is also affected by other settings such as conditional formatting, list objects, etc., then the display style may be different from [GetStyle()](../getstyle()/). <br></br>For flags of adjusting borders according to adjacent cells, [BorderType.TopBorder](../bordertype.topborder/)/[BorderType.BottomBorder](../bordertype.bottomborder/) [BorderType.LeftBorder](../bordertype.leftborder/)/[BorderType.RightBorder](../bordertype.rightborder/) denote whether check and combine the bottom/top/right/left borders of the left/right/top/bottom cells adjacent to this one. <br></br>For performance and compatibility consideration, some enums are used to denote some special operations: <br></br>[BorderType.Horizontal](../bordertype.horizontal/)/[BorderType.Vertical](../bordertype.vertical/) denote whether check and combine the bottom/right border of merged cells to this one. <br></br>[BorderType.Diagonal](../bordertype.diagonal/)(that is, both [StyleModifyFlag.DiagonalUpBorder](../stylemodifyflag.diagonalupborder/) and [StyleModifyFlag.DiagonalDownBorder](../stylemodifyflag.diagonaldownborder/) have been set) denotes check and combine borders from the display style of adjacent cells. <br></br>Please note, checking borders/styles of adjacent cells, especially the display styles, is time-consumed process. If there is no need to get the borders for the returned style, using [BorderType.None](../bordertype.none/) to disable the process of adjacent cells will give better performance. When getting borders of adjacent cells from styles defined on those cells only(without setting [BorderType.Diagonal](../bordertype.diagonal/)), the performance also may be better because checking the display style of one cell is time-consumed too.

### getFormatConditions() {#getFormatConditions--}

Gets format conditions which applies to this cell.

```javascript
getFormatConditions() : FormatConditionCollection[];
```


**Returns**

Returns [FormatConditionCollection](../formatconditioncollection/) object

### getStyle() {#getStyle--}

Gets the cell style.

```javascript
getStyle() : Style;
```


**Returns**

Style object.

**Remarks**

To change the style of the cell, please call Cell.SetStyle() method after modifying the returned style object. This method is same with [GetStyle(bool)](../getstyle(bool)/) with true value for the parameter.

### getStyle(boolean) {#getStyle-boolean-}

If checkBorders is true, check whether other cells' borders will effect the style of this cell.

```javascript
getStyle(checkBorders: boolean) : Style;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| checkBorders | boolean | Check other cells' borders |

**Returns**

Style object.

### setStyle(Style) {#setStyle-style-}

Sets the cell style.

```javascript
setStyle(style: Style) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../style/) | The cell style. |

**Remarks**

If the border settings are changed, the border of adjust cells will be updated too.

### setStyle(Style, boolean) {#setStyle-style-boolean-}

Apply the changed property of style to the cell.

```javascript
setStyle(style: Style, explicitFlag: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../style/) | The cell style. |
| explicitFlag | boolean | True, only overwriting formatting which is explicitly set. |

### setStyle(Style, StyleFlag) {#setStyle-style-styleflag-}

Apply the cell style based on flags.

```javascript
setStyle(style: Style, flag: StyleFlag) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../style/) | The cell style. |
| flag | [StyleFlag](../styleflag/) | The style flag. |

### setFormula(string, Object) {#setFormula-string-object-}

Set the formula and the value(calculated result) of the formula.

```javascript
setFormula(formula: string, value: Object) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | The formula. |
| value | Object | The value(calculated result) of the formula. |

### setFormula(string, FormulaParseOptions) {#setFormula-string-formulaparseoptions-}

Set the formula and the value(calculated result) of the formula.

```javascript
setFormula(formula: string, options: FormulaParseOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | The formula. |
| options | [FormulaParseOptions](../formulaparseoptions/) | Options for parsing the formula. |

### setFormula(string, FormulaParseOptions, Object) {#setFormula-string-formulaparseoptions-object-}

Set the formula and the value(calculated result) of the formula.

```javascript
setFormula(formula: string, options: FormulaParseOptions, value: Object) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | The formula. |
| options | [FormulaParseOptions](../formulaparseoptions/) | Options for parsing the formula. |
| value | Object | The value(calculated result) of the formula. |

### getFormula(boolean, boolean) {#getFormula-boolean-boolean-}

Get the formula of this cell.

```javascript
getFormula(isR1C1: boolean, isLocal: boolean) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns**

the formula of this cell.

### setArrayFormula(string, number, number) {#setArrayFormula-string-number-number-}

Sets an array formula(legacy array formula entered via CTRL+SHIFT+ENTER in ms excel) to a range of cells.

```javascript
setArrayFormula(arrayFormula: string, rowNumber: number, columnNumber: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | string | Array formula. |
| rowNumber | number | Number of rows to populate result of the array formula. |
| columnNumber | number | Number of columns to populate result of the array formula. |

### setArrayFormula(string, number, number, FormulaParseOptions) {#setArrayFormula-string-number-number-formulaparseoptions-}

Sets an array formula to a range of cells.

```javascript
setArrayFormula(arrayFormula: string, rowNumber: number, columnNumber: number, options: FormulaParseOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | string | Array formula. |
| rowNumber | number | Number of rows to populate result of the array formula. |
| columnNumber | number | Number of columns to populate result of the array formula. |
| options | [FormulaParseOptions](../formulaparseoptions/) | Options for parsing the formula. |

### setArrayFormula(string, number, number, FormulaParseOptions, Object[][]) {#setArrayFormula-string-number-number-formulaparseoptions-objectarrayarray-}

Sets an array formula to a range of cells.

```javascript
setArrayFormula(arrayFormula: string, rowNumber: number, columnNumber: number, options: FormulaParseOptions, values: Object[][]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | string | Array formula. |
| rowNumber | number | Number of rows to populate result of the array formula. |
| columnNumber | number | Number of columns to populate result of the array formula. |
| options | [FormulaParseOptions](../formulaparseoptions/) | Options for parsing the formula. |
| values | Object[][] | values for those cells with given array formula |

### setSharedFormula(string, number, number) {#setSharedFormula-string-number-number-}

Sets shared formulas to a range of cells.

```javascript
setSharedFormula(sharedFormula: string, rowNumber: number, columnNumber: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sharedFormula | string | Shared formula. |
| rowNumber | number | Number of rows to populate the formula. |
| columnNumber | number | Number of columns to populate the formula. |

### setSharedFormula(string, number, number, FormulaParseOptions) {#setSharedFormula-string-number-number-formulaparseoptions-}

Sets shared formulas to a range of cells.

```javascript
setSharedFormula(sharedFormula: string, rowNumber: number, columnNumber: number, options: FormulaParseOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sharedFormula | string | Shared formula. |
| rowNumber | number | Number of rows to populate the formula. |
| columnNumber | number | Number of columns to populate the formula. |
| options | [FormulaParseOptions](../formulaparseoptions/) | Options for parsing the formula. |

### setSharedFormula(string, number, number, FormulaParseOptions, Object[][]) {#setSharedFormula-string-number-number-formulaparseoptions-objectarrayarray-}

Sets shared formulas to a range of cells.

```javascript
setSharedFormula(sharedFormula: string, rowNumber: number, columnNumber: number, options: FormulaParseOptions, values: Object[][]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sharedFormula | string | Shared formula. |
| rowNumber | number | Number of rows to populate the formula. |
| columnNumber | number | Number of columns to populate the formula. |
| options | [FormulaParseOptions](../formulaparseoptions/) | Options for parsing the formula. |
| values | Object[][] | values for those cells with given shared formula |

### getPrecedents() {#getPrecedents--}

Gets all references appearing in this cell's formula.

```javascript
getPrecedents() : ReferredAreaCollection;
```


**Returns**

Collection of all references appearing in this cell's formula.

**Remarks**

ul> <li>Returns null if this is not a formula cell.</li> <li>All references appearing in this cell's formula will be returned no matter they are referenced or not while calculating. For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating, it is still taken as the formula's precedents.</li> <li>To get those references which influence the calculation only, please use [GetPrecedentsInCalculation()](../getprecedentsincalculation()/).</li> </ul

**Example**
```javascript
const { Workbook, CellsHelper } = require("aspose.cells.node");

var workbook = new Workbook();
var cells = workbook.getWorksheets().get(0).getCells();
cells.get("A1").setFormula("= B1 + SUM(B1:B10)");
var areas = cells.get("A1").getPrecedents();
for (var i = 0; i < areas.getCount(); i++) {
    var area = areas.get(i);
    var stringBuilder = "";
    if (area.isExternalLink()) {
        stringBuilder += "[";
        stringBuilder += area.getExternalFileName();
        stringBuilder += "]";
    }
    stringBuilder += area.getSheetName();
    stringBuilder += "!";
    stringBuilder += CellsHelper.cellIndexToName(area.getStartRow(), area.getStartColumn());
    if (area.isArea()) {
        stringBuilder += ":";
        stringBuilder += CellsHelper.cellIndexToName(area.getEndRow(), area.getEndColumn());
    }
}
workbook.save("output/CellGetPrecedents.xls");
```

### getDependents(boolean) {#getDependents-boolean-}

Get all cells whose formula references to this cell directly.

```javascript
getDependents(isAll: boolean) : Cell[];
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isAll | boolean | Indicates whether check formulas in other worksheets |

**Returns**

[Cell](../cell/)[]

**Remarks**

ul> <li>If one reference containing this cell appears in one cell's formula, that cell will be taken as the dependent of this cell, no matter the reference or this cell is used or not while calculating. For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating, this formula is still be taken as A2's dependent. </li> <li>To get those formulas whose calculated results depend on this cell, please use [GetDependentsInCalculation(bool)](../getdependentsincalculation(bool)/).</li> <li>When tracing dependents for one cell, all formulas in the workbook or worksheet will be analized and checked. So it is a time consumed process. If user need to trace dependents for lots of cells, using this method will cause poor performance. For performance consideration, user should use [GetDependentsInCalculation(bool)](../getdependentsincalculation(bool)/) instead. Or, user may gather precedents map of all cells by [GetPrecedents()](../getprecedents()/) firstly, and then build the dependents map according to the precedents map.</li> </ul

### getPrecedentsInCalculation() {#getPrecedentsInCalculation--}

Gets all precedents(reference to cells in current workbook) used by this cell's formula while calculating it.

```javascript
getPrecedentsInCalculation() : ReferredAreaEnumerator;
```


**Returns**

Enumerator to enumerate all references(ReferredArea)

**Remarks**

This method can only work with the situation that [FormulaSettings.EnableCalculationChain](../formulasettings.enablecalculationchain/) is true for the workbook and the workbook has been fully calculated. If this cell is not a formula or it does not reference to any other cells, null will be returned.

### getDependentsInCalculation(boolean) {#getDependentsInCalculation-boolean-}

Gets all cells whose calculated result depends on this cell.

```javascript
getDependentsInCalculation(recursive: boolean) : CellEnumerator;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| recursive | boolean | Whether returns those dependents which do not reference to this cell directly         /// but reference to other leafs of this cell |

**Returns**

Enumerator to enumerate all dependents(Cell objects)

**Remarks**

To use this method, please make sure the workbook has been set with true value for [FormulaSettings.EnableCalculationChain](../formulasettings.enablecalculationchain/) and has been fully calculated with this setting. If there is no formula reference to this cell, null will be returned.

### getArrayRange() {#getArrayRange--}

Gets the array range if the cell's formula is an array formula.

```javascript
getArrayRange() : CellArea;
```


**Returns**

The array range.

**Remarks**

Only applies when the cell's formula is an array formula

### setDynamicArrayFormula(string, FormulaParseOptions, boolean) {#setDynamicArrayFormula-string-formulaparseoptions-boolean-}

Sets dynamic array formula and make the formula spill into neighboring cells if possible.

```javascript
setDynamicArrayFormula(arrayFormula: string, options: FormulaParseOptions, calculateValue: boolean) : CellArea;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | string | the formula expression |
| options | [FormulaParseOptions](../formulaparseoptions/) | options to parse formula.         /// "Parse" option will be ignored and the formula will always be parsed immediately |
| calculateValue | boolean | whether calculate this dynamic array formula for those cells in the spilled range. |

**Returns**

the range that the formula should spill into.

**Remarks**

the returned range may be not same with the actual one that this dynamic array formula spills into. If there are non-empty cells in the range, the formula will be set for current cell only and marked as "#SPILL!". But for such kind of situation we still return the whole range that this formula should spill into.

### setDynamicArrayFormula(string, FormulaParseOptions, Object[][], boolean, boolean) {#setDynamicArrayFormula-string-formulaparseoptions-objectarrayarray-boolean-boolean-}

Sets dynamic array formula and make the formula spill into neighboring cells if possible.

```javascript
setDynamicArrayFormula(arrayFormula: string, options: FormulaParseOptions, values: Object[][], calculateRange: boolean, calculateValue: boolean) : CellArea;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | string | the formula expression |
| options | [FormulaParseOptions](../formulaparseoptions/) | options to parse formula.         /// "Parse" option will be ignored and the formula will always be parsed immediately |
| values | Object[][] | values(calculated results) for those cells with given dynamic array formula |
| calculateRange | boolean | Whether calculate the spilled range for this dynamic array formula.         /// If the "values" parameter is not null and this flag is false,         /// then the spilled range's height will be values.Length and width will be values[0].Length. |
| calculateValue | boolean | whether calculate this dynamic array formula for those cells in the spilled range when "values" is null         /// or corresponding item in "values" for one cell is null. |

**Returns**

the range that the formula should spill into.

**Remarks**

the returned range may be not same with the actual one that this dynamic array formula spills into. If there are non-empty cells in the range, the formula will be set for current cell only and marked as "#SPILL!". But for such kind of situation we still return the whole range that this formula should spill into.

### setDynamicArrayFormula(string, FormulaParseOptions, Object[][], boolean, boolean, CalculationOptions) {#setDynamicArrayFormula-string-formulaparseoptions-objectarrayarray-boolean-boolean-calculationoptions-}

Sets dynamic array formula and make the formula spill into neighboring cells if possible.

```javascript
setDynamicArrayFormula(arrayFormula: string, options: FormulaParseOptions, values: Object[][], calculateRange: boolean, calculateValue: boolean, copts: CalculationOptions) : CellArea;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | string | the formula expression |
| options | [FormulaParseOptions](../formulaparseoptions/) | options to parse formula.         /// "Parse" option will be ignored and the formula will always be parsed immediately |
| values | Object[][] | values(calculated results) for those cells with given dynamic array formula |
| calculateRange | boolean | Whether calculate the spilled range for this dynamic array formula.         /// If the "values" parameter is not null and this flag is false,         /// then the spilled range's height will be values.Length and width will be values[0].Length. |
| calculateValue | boolean | whether calculate this dynamic array formula for those cells in the spilled range when "values" is null         /// or corresponding item in "values" for one cell is null. |
| copts | [CalculationOptions](../calculationoptions/) | The options for calculating formula.         /// Commonly, for performance consideration, the [CalculationOptions.Recursive](../calculationoptions.recursive/) property should be false. |

**Returns**

the range that the formula should spill into.

**Remarks**

the returned range may be not same with the actual one that this dynamic array formula spills into. If there are non-empty cells in the range, the formula will be set for current cell only and marked as "#SPILL!". But for such kind of situation we still return the whole range that this formula should spill into.

### setTableFormula(number, number, string, string, Object[][]) {#setTableFormula-number-number-string-string-objectarrayarray-}

Create two-variable data table for given range starting from this cell.

```javascript
setTableFormula(rowNumber: number, columnNumber: number, rowInputCell: string, columnInputCell: string, values: Object[][]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowNumber | number | Number of rows to populate the formula. |
| columnNumber | number | Number of columns to populate the formula. |
| rowInputCell | string | the row input cell |
| columnInputCell | string | the column input cell |
| values | Object[][] | values for cells in table formula range |

### setTableFormula(number, number, string, boolean, Object[][]) {#setTableFormula-number-number-string-boolean-objectarrayarray-}

Create one-variable data table for given range starting from this cell.

```javascript
setTableFormula(rowNumber: number, columnNumber: number, inputCell: string, isRowInput: boolean, values: Object[][]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowNumber | number | Number of rows to populate the formula. |
| columnNumber | number | Number of columns to populate the formula. |
| inputCell | string | the input cell |
| isRowInput | boolean | Indicates whether the input cell is a row input cell(true) or a column input cell(false). |
| values | Object[][] | values for cells in table formula range |

### setTableFormula(number, number, number, number, number, number, Object[][]) {#setTableFormula-number-number-number-number-number-number-objectarrayarray-}

Create two-variable data table for given range starting from this cell.

```javascript
setTableFormula(rowNumber: number, columnNumber: number, rowIndexOfRowInputCell: number, columnIndexOfRowInputCell: number, rowIndexOfColumnInputCell: number, columnIndexOfColumnInputCell: number, values: Object[][]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowNumber | number | Number of rows to populate the formula. |
| columnNumber | number | Number of columns to populate the formula. |
| rowIndexOfRowInputCell | number | row index of the row input cell |
| columnIndexOfRowInputCell | number | column index of the row input cell |
| rowIndexOfColumnInputCell | number | row index of the column input cell |
| columnIndexOfColumnInputCell | number | column index of the column input cell |
| values | Object[][] | values for cells in table formula range |

### setTableFormula(number, number, number, number, boolean, Object[][]) {#setTableFormula-number-number-number-number-boolean-objectarrayarray-}

Create one-variable data table for given range starting from this cell.

```javascript
setTableFormula(rowNumber: number, columnNumber: number, rowIndexOfInputCell: number, columnIndexOfInputCell: number, isRowInput: boolean, values: Object[][]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowNumber | number | Number of rows to populate the formula. |
| columnNumber | number | Number of columns to populate the formula. |
| rowIndexOfInputCell | number | row index of the input cell |
| columnIndexOfInputCell | number | column index of the input cell |
| isRowInput | boolean | Indicates whether the input cell is a row input cell(true) or a column input cell(false). |
| values | Object[][] | values for cells in table formula range |

### removeArrayFormula(boolean) {#removeArrayFormula-boolean-}

Remove array formula.

```javascript
removeArrayFormula(leaveNormalFormula: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| leaveNormalFormula | boolean | True represents converting the array formula to normal formula. |

### copy(Cell) {#copy-cell-}

Copies data from a source cell.

```javascript
copy(cell: Cell) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cell | [Cell](../cell/) | Source [Cell](../cell/) object. |

### characters(number, number) {#characters-number-number-}

Returns a Characters object that represents a range of characters within the cell text.

```javascript
characters(startIndex: number, length: number) : FontSetting;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | number | The index of the start of the character. |
| length | number | The number of characters. |

**Returns**

Characters object.

**Remarks**

This method only works on cell with string value.

**Example**
```javascript
const { Workbook, Color } = require("aspose.cells.node");

var excel = new Workbook();
excel.getWorksheets().get(0).getCells().get("A1").putValue("Helloworld");
excel.getWorksheets().get(0).getCells().get("A1").characters(5, 5).getFont().setIsBold(true);
excel.getWorksheets().get(0).getCells().get("A1").characters(5, 5).getFont().setColor(Color.Blue);
```

### replace(string, string, ReplaceOptions) {#replace-string-string-replaceoptions-}

Replace text of the cell with options.

```javascript
replace(placeHolder: string, newValue: string, options: ReplaceOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | string | Cell placeholder |
| newValue | string | String value to replace |
| options | [ReplaceOptions](../replaceoptions/) | The replace options |

### insertText(number, string) {#insertText-number-string-}

Insert some characters to the cell. If the cell is rich formatted, this method could keep the original formatting.

```javascript
insertText(index: number, text: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
| text | string | Inserted text. |

### isRichText() {#isRichText--}

Indicates whether the string value of this cell is a rich formatted text.

```javascript
isRichText() : boolean;
```


### getCharacters() {#getCharacters--}

Returns all Characters objects that represents a range of characters within the cell text.

```javascript
getCharacters() : FontSetting[];
```


**Returns**

All Characters objects

### getCharacters(boolean) {#getCharacters-boolean-}

Returns all Characters objects that represents a range of characters within the cell text.

```javascript
getCharacters(flag: boolean) : FontSetting[];
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| flag | boolean | Indicates whether applying table style to the cell if the cell is in the table. |

**Returns**

All Characters objects

### setCharacters(FontSetting[]) {#setCharacters-fontsettingarray-}

Sets rich text format of the cell.

```javascript
setCharacters(characters: FontSetting[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| characters | [FontSetting](../fontsetting/)[] | All Characters objects. |

### getMergedRange() {#getMergedRange--}

Returns a [Range](../range/) object which represents a merged range.

```javascript
getMergedRange() : Range;
```


**Returns**

[Range](../range/) object. Null if this cell is not merged.

### getHtmlString(boolean) {#getHtmlString-boolean-}

Gets the html string which contains data and some formats in this cell.

```javascript
getHtmlString(html5: boolean) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| html5 | boolean | Indicates whether the value is compatible for html5 |

### toString() {#toString--}

Returns a string represents the current Cell object.

```javascript
toString() : string;
```


### toJson() {#toJson--}

Convert [Cell](../cell/) to JSON struct data.

```javascript
toJson() : string;
```


### equals(Object) {#equals-object-}

Checks whether this object refers to the same cell with another.

```javascript
equals(obj: Object) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | another object |

**Returns**

true if two objects refers to the same cell.

### equals(Cell) {#equals-cell-}

Checks whether this object refers to the same cell with another cell object.

```javascript
equals(cell: Cell) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cell | [Cell](../cell/) | another cell object |

**Returns**

true if two cell objects refers to the same cell.

### getHashCode() {#getHashCode--}

Serves as a hash function for a particular type.

```javascript
getHashCode() : number;
```


**Returns**

A hash code for current Cell object.

### getConditionalFormattingResult() {#getConditionalFormattingResult--}

Get the result of the conditional formatting.

```javascript
getConditionalFormattingResult() : ConditionalFormattingResult;
```


**Returns**

[ConditionalFormattingResult](../conditionalformattingresult/)

**Remarks**

Returns null if no conditional formatting is applied to this cell,

### getValidation() {#getValidation--}

Gets the validation applied to this cell.

```javascript
getValidation() : Validation;
```


**Returns**

[Validation](../validation/)

### getValidationValue() {#getValidationValue--}

Gets the value of validation which applied to this cell.

```javascript
getValidationValue() : boolean;
```


### getTable() {#getTable--}

Gets the table which contains this cell.

```javascript
getTable() : ListObject;
```


**Returns**

[ListObject](../listobject/)

### getRichValue() {#getRichValue--}

Gets rich value of the cell.

```javascript
getRichValue() : CellRichValue;
```


**Returns**

[CellRichValue](../cellrichvalue/)

### dispose() {#dispose--}



```javascript
dispose() : void;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



