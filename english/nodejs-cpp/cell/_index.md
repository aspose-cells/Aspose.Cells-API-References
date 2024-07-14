---
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


## Methods

| Method | Description |
| --- | --- |
| [getWorksheet()](#getWorksheet--)| Gets the parent worksheet. |
| [getDateTimeValue()](#getDateTimeValue--)| Gets the DateTime value contained in the cell. |
| [getRow()](#getRow--)| Gets row number (zero based) of the cell. |
| [getColumn()](#getColumn--)| Gets column number (zero based) of the cell. |
| [isFormula()](#isFormula--)| Represents if the specified cell contains formula. |
| [getType()](#getType--)| Represents cell value type. |
| [getName()](#getName--)| Gets the name of the cell. |
| [isErrorValue()](#isErrorValue--)| Checks if the value of this cell is an error. |
| [isNumericValue()](#isNumericValue--)| Indicates whether the value of this cell is numeric(int, double and datetime) |
| [getNumberCategoryType()](#getNumberCategoryType--)| Represents the category type of this cell's number formatting. |
| [getDisplayStringValue()](#getDisplayStringValue--)| Gets the formatted string value of this cell by cell's display style. |
| [getIntValue()](#getIntValue--)| Gets the integer value contained in the cell. |
| [getDoubleValue()](#getDoubleValue--)| Gets the double value contained in the cell. |
| [getFloatValue()](#getFloatValue--)| Gets the float value contained in the cell. |
| [getBoolValue()](#getBoolValue--)| Gets the boolean value contained in the cell. |
| [getHasCustomStyle()](#getHasCustomStyle--)| Indicates whether this cell has custom style settings(different from the default one inherited from corresponding row, column, or workbook). |
| [getSharedStyleIndex()](#getSharedStyleIndex--)| Gets cell's shared style index in the style pool. |
| [setFormula(string)](#setFormula-string-)| Gets or sets a formula of the [Cell](/nodejs-cpp/cell/). |
| [getFormulaLocal()](#getFormulaLocal--)| Get the locale formatted formula of the cell. |
| [setFormulaLocal(string)](#setFormulaLocal-string-)| Get the locale formatted formula of the cell. |
| [getR1C1Formula()](#getR1C1Formula--)| Gets or sets a R1C1 formula of the [Cell](/nodejs-cpp/cell/). |
| [setR1C1Formula(string)](#setR1C1Formula-string-)| Gets or sets a R1C1 formula of the [Cell](/nodejs-cpp/cell/). |
| [getContainsExternalLink()](#getContainsExternalLink--)| Indicates whether this cell contains an external link. Only applies when the cell is a formula cell. |
| [isArrayHeader()](#isArrayHeader--)| Indicates the cell's formula is an array formula and it is the first cell of the array. |
| [isDynamicArrayFormula()](#isDynamicArrayFormula--)| Indicates whether the cell's formula is dynamic array formula(true) or legacy array formula(false). |
| [isArrayFormula()](#isArrayFormula--)| Indicates whether the cell formula is an array formula. |
| [isSharedFormula()](#isSharedFormula--)| Indicates whether the cell formula is part of shared formula. |
| [isTableFormula()](#isTableFormula--)| Indicates whether this cell is part of table formula. |
| [isStyleSet()](#isStyleSet--)| Indicates if the cell's style is set. If return false, it means this cell has a default cell format. |
| [isMerged()](#isMerged--)| Checks if a cell is part of a merged range or not. |
| [getComment()](#getComment--)| Gets the comment of this cell. |
| [setHtmlString(string)](#setHtmlString-string-)| Gets and sets the html string which contains data and some formats in this cell. |
| [getEmbeddedImage()](#getEmbeddedImage--)| Gets and sets the embeddedn image in the cell. |
| [setEmbeddedImage(number[])](#setEmbeddedImage-numberarray-)| Gets and sets the embeddedn image in the cell. |
| [calculate(CalculationOptions)](#calculate-calculationoptions-)| Calculates the formula of the cell. |
| [putValue(boolean)](#putValue-boolean-)| Puts a boolean value into the cell. |
| [putValue(number)](#putValue-number-)| Puts an integer value into the cell. |
| [putValue(number)](#putValue-number-)| Puts a double value into the cell. |
| [putValue(string, boolean, boolean)](#putValue-string-boolean-boolean-)| Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will be reset. |
| [putValue(string, boolean)](#putValue-string-boolean-)| Puts a string value into the cell and converts the value to other data type if appropriate. |
| [putValue(string)](#putValue-string-)| Puts a string value into the cell. |
| [putValue(Date)](#putValue-date-)| Puts a DateTime value into the cell. |
| [getStringValue(CellValueFormatStrategy)](#getStringValue-cellvalueformatstrategy-)| Gets the string value by specific formatted strategy. |
| [getWidthOfValue()](#getWidthOfValue--)| Gets the width of the value in unit of pixels. |
| [getHeightOfValue()](#getHeightOfValue--)| Gets the height of the value in unit of pixels. |
| [getDisplayStyle()](#getDisplayStyle--)| Gets the display style of the cell. If this cell is also affected by other settings such as conditional formatting, list objects, etc., then the display style may be different from cell.GetStyle(). |
| [getDisplayStyle(boolean)](#getDisplayStyle-boolean-)| Gets the display style of the cell. If the cell is conditional formatted, the display style is not same as the cell.GetStyle(). |
| [getFormatConditions()](#getFormatConditions--)| Gets format conditions which applies to this cell. |
| [getStyle()](#getStyle--)| Gets the cell style. |
| [getStyle(boolean)](#getStyle-boolean-)| If checkBorders is true, check whether other cells' borders will effect the style of this cell. |
| [setStyle(Style)](#setStyle-style-)| Sets the cell style. |
| [setStyle(Style, boolean)](#setStyle-style-boolean-)| Apply the changed property of style to the cell. |
| [setStyle(Style, StyleFlag)](#setStyle-style-styleflag-)| Apply the cell style based on flags. |
| [getFormula(boolean, boolean)](#getFormula-boolean-boolean-)| Get the formula of this cell. |
| [setArrayFormula(string, number, number)](#setArrayFormula-string-number-number-)| Sets an array formula(legacy array formula entered via CTRL+SHIFT+ENTER in ms excel) to a range of cells. |
| [setArrayFormula(string, number, number, FormulaParseOptions)](#setArrayFormula-string-number-number-formulaparseoptions-)| Sets an array formula to a range of cells. |
| [setSharedFormula(string, number, number)](#setSharedFormula-string-number-number-)| Sets shared formulas to a range of cells. |
| [setSharedFormula(string, number, number, FormulaParseOptions)](#setSharedFormula-string-number-number-formulaparseoptions-)| Sets shared formulas to a range of cells. |
| [getPrecedents()](#getPrecedents--)| Gets all references appearing in this cell's formula. |
| [getDependents(boolean)](#getDependents-boolean-)| Get all cells whose formula references to this cell directly. |
| [getPrecedentsInCalculation()](#getPrecedentsInCalculation--)| Gets all precedents(reference to cells in current workbook) used by this cell's formula while calculating it. |
| [getDependentsInCalculation(boolean)](#getDependentsInCalculation-boolean-)| Gets all cells whose calculated result depends on this cell. |
| [getArrayRange()](#getArrayRange--)| Gets the array range if the cell's formula is an array formula. |
| [setDynamicArrayFormula(string, FormulaParseOptions, boolean)](#setDynamicArrayFormula-string-formulaparseoptions-boolean-)| Sets dynamic array formula and make the formula spill into neighboring cells if possible. |
| [removeArrayFormula(boolean)](#removeArrayFormula-boolean-)| Remove array formula. |
| [copy(Cell)](#copy-cell-)| Copies data from a source cell. |
| [characters(number, number)](#characters-number-number-)| Returns a Characters object that represents a range of characters within the cell text. |
| [replace(string, string, ReplaceOptions)](#replace-string-string-replaceoptions-)| Replace text of the cell with options. |
| [insertText(number, string)](#insertText-number-string-)| Insert some characters to the cell. If the cell is rich formatted, this method could keep the original formatting. |
| [isRichText()](#isRichText--)| Indicates whether the string value of this cell is a rich formatted text. |
| [getCharacters()](#getCharacters--)| Returns all Characters objects that represents a range of characters within the cell text. |
| [getCharacters(boolean)](#getCharacters-boolean-)| Returns all Characters objects that represents a range of characters within the cell text. |
| [setCharacters(FontSetting[])](#setCharacters-fontsettingarray-)| Sets rich text format of the cell. |
| [getMergedRange()](#getMergedRange--)| Returns a [Range](/nodejs-cpp/range/) object which represents a merged range. |
| [getHtmlString(boolean)](#getHtmlString-boolean-)| Gets the html string which contains data and some formats in this cell. |
| [toString()](#toString--)| Returns a string represents the current Cell object. |
| [toJson()](#toJson--)| Convert [Cell](/nodejs-cpp/cell/) to JSON struct data. |
| [getHashCode()](#getHashCode--)| Serves as a hash function for a particular type. |
| [equals(Cell)](#equals-cell-)| Checks whether this object refers to the same cell with another cell object. |
| [getConditionalFormattingResult()](#getConditionalFormattingResult--)| Get the result of the conditional formatting. |
| [getValidation()](#getValidation--)| Gets the validation applied to this cell. |
| [getValidationValue()](#getValidationValue--)| Gets the value of validation which applied to this cell. |
| [getTable()](#getTable--)| Gets the table which contains this cell. |
| [dispose()](#dispose--)|  |


### getWorksheet() {#getWorksheet--}

Gets the parent worksheet.

```javascript
getWorksheet() : Worksheet;
```


**Returns**

[Worksheet](/nodejs-cpp/worksheet/)

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


### getType() {#getType--}

Represents cell value type.

```javascript
getType() : CellValueType;
```


**Returns**

[CellValueType](/nodejs-cpp/cellvaluetype/)

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

### getNumberCategoryType() {#getNumberCategoryType--}

Represents the category type of this cell's number formatting.

```javascript
getNumberCategoryType() : NumberCategoryType;
```


**Returns**

[NumberCategoryType](/nodejs-cpp/numbercategorytype/)

**Remarks**

When cell's formatting pattern is combined with conditional formatting patterns, then the returned type is corresponding to the part which is used for current value of this cell. For example, if the formatting pattern for this cell is "#,##0;(#,##0);"-";@", then when cell's value is numeric and not 0, the returned type is [NumberCategoryType.Number](/nodejs-cpp/numbercategorytype.number/); When cell's value is 0 or not numeric value, the returned type is [NumberCategoryType.Text](/nodejs-cpp/numbercategorytype.text/).

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


### setFormula(string) {#setFormula-string-}

Gets or sets a formula of the [Cell](/nodejs-cpp/cell/).

```javascript
setFormula(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

A formula string always begins with an equal sign (=). And please always use comma(,) as parameters delimiter, such as "=SUM(A1, E1, H2)".

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

Gets or sets a R1C1 formula of the [Cell](/nodejs-cpp/cell/).

```javascript
getR1C1Formula() : string;
```


### setR1C1Formula(string) {#setR1C1Formula-string-}

Gets or sets a R1C1 formula of the [Cell](/nodejs-cpp/cell/).

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

[Comment](/nodejs-cpp/comment/)

**Remarks**

If there is no comment applies to the cell, returns null.

### setHtmlString(string) {#setHtmlString-string-}

Gets and sets the html string which contains data and some formats in this cell.

```javascript
setHtmlString(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getEmbeddedImage() {#getEmbeddedImage--}

Gets and sets the embeddedn image in the cell.

```javascript
getEmbeddedImage() : number[];
```


**Returns**

number[]

### setEmbeddedImage(number[]) {#setEmbeddedImage-numberarray-}

Gets and sets the embeddedn image in the cell.

```javascript
setEmbeddedImage(value: number[]) : void;
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
| options | [CalculationOptions](/nodejs-cpp/calculationoptions/) | Options for calculation |

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

### getStringValue(CellValueFormatStrategy) {#getStringValue-cellvalueformatstrategy-}

Gets the string value by specific formatted strategy.

```javascript
getStringValue(formatStrategy: CellValueFormatStrategy) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formatStrategy | [CellValueFormatStrategy](/nodejs-cpp/cellvalueformatstrategy/) | The formatted strategy. |

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

Gets the display style of the cell. If this cell is also affected by other settings such as conditional formatting, list objects, etc., then the display style may be different from cell.GetStyle().

```javascript
getDisplayStyle() : Style;
```


**Returns**

[Style](/nodejs-cpp/style/)

### getDisplayStyle(boolean) {#getDisplayStyle-boolean-}

Gets the display style of the cell. If the cell is conditional formatted, the display style is not same as the cell.GetStyle().

```javascript
getDisplayStyle(includeMergedBorders: boolean) : Style;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| includeMergedBorders | boolean | Indicates whether checking borders of the merged cells. |

**Returns**

[Style](/nodejs-cpp/style/)

### getFormatConditions() {#getFormatConditions--}

Gets format conditions which applies to this cell.

```javascript
getFormatConditions() : FormatConditionCollection[];
```


**Returns**

Returns [FormatConditionCollection](/nodejs-cpp/formatconditioncollection/) object

### getStyle() {#getStyle--}

Gets the cell style.

```javascript
getStyle() : Style;
```


**Returns**

Style object.

**Remarks**

To change the style of the cell, please call Cell.SetStyle() method after modifying the returned style object. This method is same with [GetStyle(bool)](/nodejs-cpp/getstyle(bool)/) with true value for the parameter.

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
| style | [Style](/nodejs-cpp/style/) | The cell style. |

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
| style | [Style](/nodejs-cpp/style/) | The cell style. |
| explicitFlag | boolean | True, only overwriting formatting which is explicitly set. |

### setStyle(Style, StyleFlag) {#setStyle-style-styleflag-}

Apply the cell style based on flags.

```javascript
setStyle(style: Style, flag: StyleFlag) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](/nodejs-cpp/style/) | The cell style. |
| flag | [StyleFlag](/nodejs-cpp/styleflag/) | The style flag. |

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
| options | [FormulaParseOptions](/nodejs-cpp/formulaparseoptions/) | Options for parsing the formula. |

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
| options | [FormulaParseOptions](/nodejs-cpp/formulaparseoptions/) | Options for parsing the formula. |

### getPrecedents() {#getPrecedents--}

Gets all references appearing in this cell's formula.

```javascript
getPrecedents() : ReferredAreaCollection;
```


**Returns**

Collection of all references appearing in this cell's formula.

**Remarks**

<ul> <li>Returns null if this is not a formula cell.</li> <li>All references appearing in this cell's formula will be returned no matter they are referenced or not while calculating. For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating, it is still taken as the formula's precedents.</li> <li>To get those references which influence the calculation only, please use [GetPrecedentsInCalculation()](/nodejs-cpp/getprecedentsincalculation()/).</li> </ul>

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

[Cell](/nodejs-cpp/cell/)[]

**Remarks**

<ul> <li>If one reference containing this cell appears in one cell's formula, that cell will be taken as the dependent of this cell, no matter the reference or this cell is used or not while calculating. For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating, this formula is still be taken as A2's dependent. </li> <li>To get those formulas whose calculated results depend on this cell, please use [GetDependentsInCalculation(bool)](/nodejs-cpp/getdependentsincalculation(bool)/).</li> <li>When tracing dependents for one cell, all formulas in the workbook or worksheet will be analized and checked. So it is a time consumed process. If user need to trace dependents for lots of cells, using this method will cause poor performance. For performance consideration, user should use [GetDependentsInCalculation(bool)](/nodejs-cpp/getdependentsincalculation(bool)/) instead. Or, user may gather precedents map of all cells by [GetPrecedents()](/nodejs-cpp/getprecedents()/) firstly, and then build the dependents map according to the precedents map.</li> </ul>

### getPrecedentsInCalculation() {#getPrecedentsInCalculation--}

Gets all precedents(reference to cells in current workbook) used by this cell's formula while calculating it.

```javascript
getPrecedentsInCalculation() : ReferredAreaEnumerator;
```


**Returns**

Enumerator to enumerate all references(ReferredArea)

**Remarks**

This method can only work with the situation that [FormulaSettings.EnableCalculationChain](/nodejs-cpp/formulasettings.enablecalculationchain/) is true for the workbook and the workbook has been fully calculated. If this cell is not a formula or it does not reference to any other cells, null will be returned.

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

To use this method, please make sure the workbook has been set with true value for [FormulaSettings.EnableCalculationChain](/nodejs-cpp/formulasettings.enablecalculationchain/) and has been fully calculated with this setting. If there is no formula reference to this cell, null will be returned.

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
| options | [FormulaParseOptions](/nodejs-cpp/formulaparseoptions/) | options to parse formula.         /// "Parse" option will be ignored and the formula will always be parsed immediately |
| calculateValue | boolean | whether calculate this dynamic array formula for those cells in the spilled range. |

**Returns**

the range that the formula should spill into.

**Remarks**

the returned range may be not same with the actual one that this dynamic array formula spills into. If there are non-empty cells in the range, the formula will be set for current cell only and marked as "#SPILL!". But for such kind of situation we still return the whole range that this formula should spill into.

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
| cell | [Cell](/nodejs-cpp/cell/) | Source [Cell](/nodejs-cpp/cell/) object. |

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
| options | [ReplaceOptions](/nodejs-cpp/replaceoptions/) | The replace options |

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
| characters | [FontSetting](/nodejs-cpp/fontsetting/)[] | All Characters objects. |

### getMergedRange() {#getMergedRange--}

Returns a [Range](/nodejs-cpp/range/) object which represents a merged range.

```javascript
getMergedRange() : Range;
```


**Returns**

[Range](/nodejs-cpp/range/) object. Null if this cell is not merged.

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

Convert [Cell](/nodejs-cpp/cell/) to JSON struct data.

```javascript
toJson() : string;
```


### getHashCode() {#getHashCode--}

Serves as a hash function for a particular type.

```javascript
getHashCode() : number;
```


**Returns**

A hash code for current Cell object.

### equals(Cell) {#equals-cell-}

Checks whether this object refers to the same cell with another cell object.

```javascript
equals(cell: Cell) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cell | [Cell](/nodejs-cpp/cell/) | another cell object |

**Returns**

true if two cell objects refers to the same cell.

### getConditionalFormattingResult() {#getConditionalFormattingResult--}

Get the result of the conditional formatting.

```javascript
getConditionalFormattingResult() : ConditionalFormattingResult;
```


**Returns**

[ConditionalFormattingResult](/nodejs-cpp/conditionalformattingresult/)

**Remarks**

Returns null if no conditional formatting is applied to this cell,

### getValidation() {#getValidation--}

Gets the validation applied to this cell.

```javascript
getValidation() : Validation;
```


**Returns**

[Validation](/nodejs-cpp/validation/)

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

[ListObject](/nodejs-cpp/listobject/)

### dispose() {#dispose--}



```javascript
dispose() : void;
```



