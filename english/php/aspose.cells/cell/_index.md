---
title: "Cell Class"
linktitle: "Cell"
articleTitle: "Cell"
second_title: "Aspose.Cells for PHP via Java"
description: "Encapsulates the object that represents a single Workbook cell."
type: docs
weight: 530
url: /php/aspose.cells/cell/
---

## Cell class

Encapsulates the object that represents a single Workbook cell.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Worksheet](#worksheet) | Worksheet | Gets the parent worksheet. |
| [DateTimeValue](#datetimevalue) | DateTime | Gets the DateTime value contained in the cell. |
| [Row](#row) | Number | Gets row number (zero based) of the cell. |
| [Column](#column) | Number | Gets column number (zero based) of the cell. |
| [IsFormula](#isformula) | boolean | Represents if the specified cell contains formula. |
| [HasCustomFunction](#hascustomfunction) | boolean |  |
| [Type](#type) | Number | Represents cell value type. The value of the property is CellValueType integer constant. |
| [Name](#name) | String | Gets the name of the cell. A cell name includes its column letter and row number. For example, the name of a cell in row |
| [IsErrorValue](#iserrorvalue) | boolean | Checks if the value of this cell is an error. Also applies to formula cell to check whether the calculated result is an  |
| [IsNumericValue](#isnumericvalue) | boolean | Indicates whether the value of this cell is numeric(int, double and datetime) Also applies to formula cell to check the  |
| [StringValue](#stringvalue) | String | Gets the string value contained in the cell. If the type of this cell is string, then return the string value itself. Fo |
| [StringValueWithoutFormat](#stringvaluewithoutformat) | String | Gets cell's value as string without any format. NOTE: This method is now obsolete. Instead, User should get the value ob |
| [NumberCategoryType](#numbercategorytype) | Number | Represents the category type of this cell's number formatting. The value of the property is NumberCategoryType integer c |
| [DisplayStringValue](#displaystringvalue) | String | Gets the formatted string value of this cell by cell's display style. |
| [IntValue](#intvalue) | Number | Gets the integer value contained in the cell. |
| [DoubleValue](#doublevalue) | Number | Gets the double value contained in the cell. |
| [FloatValue](#floatvalue) | Number | Gets the float value contained in the cell. |
| [BoolValue](#boolvalue) | boolean | Gets the boolean value contained in the cell. |
| [HasCustomStyle](#hascustomstyle) | boolean | Indicates whether this cell has custom style settings(different from the default one inherited from corresponding row, c |
| [SharedStyleIndex](#sharedstyleindex) | Number | Gets cell's shared style index in the style pool. |
| [Formula](#formula) | String | Gets or sets a formula of the Cell . A formula string always begins with an equal sign (=). And please always use comma( |
| [FormulaLocal](#formulalocal) | String | Get the locale formatted formula of the cell. |
| [R1C1Formula](#r1c1formula) | String | Gets or sets a R1C1 formula of the Cell . |
| [ContainsExternalLink](#containsexternallink) | boolean | Indicates whether this cell contains an external link. Only applies when the cell is a formula cell. |
| [IsArrayHeader](#isarrayheader) | boolean | Indicates the cell's formula is an array formula and it is the first cell of the array. |
| [IsDynamicArrayFormula](#isdynamicarrayformula) | boolean | Indicates whether the cell's formula is dynamic array formula(true) or legacy array formula(false). |
| [IsArrayFormula](#isarrayformula) | boolean | Indicates whether the cell formula is an array formula. |
| [IsInArray](#isinarray) | boolean | Indicates whether the cell formula is an array formula. NOTE: This class is now obsolete. Instead, please use Cell.IsArr |
| [IsSharedFormula](#issharedformula) | boolean | Indicates whether the cell formula is part of shared formula. |
| [IsTableFormula](#istableformula) | boolean | Indicates whether this cell is part of table formula. |
| [IsInTable](#isintable) | boolean | Indicates whether this cell is part of table formula. NOTE: This class is now obsolete. Instead, please use Cell.IsTable |
| [Value](#value) | Object | Gets/sets the value contained in this cell. Possible type: null, Boolean, DateTime, Double, Integer String. For int valu |
| [IsStyleSet](#isstyleset) | boolean | Indicates if the cell's style is set. If return false, it means this cell has a default cell format. |
| [IsMerged](#ismerged) | boolean | Checks if a cell is part of a merged range or not. |
| [Comment](#comment) | Comment | Gets the comment of this cell. If there is no comment applies to the cell, returns null. |
| [HtmlString](#htmlstring) | String | Gets and sets the html string which contains data and some formats in this cell. |
| [IsCheckBoxStyle](#ischeckboxstyle) | boolean |  |
| [EmbeddedImage](#embeddedimage) | byte[] | Gets and sets the embeddedn image in the cell. |

## Methods

| Name | Description |
| --- | --- |
| [getArrayRange](#getarrayrange) | Gets the array range if the cell's formula is an array formula.

Only applies when the cell's formula is an array formul |
| [setDynamicArrayFormula](#setdynamicarrayformula) | Sets dynamic array formula and make the formula spill into neighboring cells if possible.

the returned range may be not |
| [setTableFormula](#settableformula) | Create two-variable data table for given range starting from this cell. |
| [removeArrayFormula](#removearrayformula) | Remove array formula. |
| [copy](#copy) | Copies data from a source cell. |
| [characters](#characters) | Returns a Characters object that represents a range of characters within the cell text.

This method only works on cell  |
| [replace](#replace) | Replace text of the cell with options. |
| [insertText](#inserttext) | Insert some characters to the cell. If the cell is rich formatted, this method could keep the original formatting. |
| [isRichText](#isrichtext) | Indicates whether the string value of this cell is a rich formatted text. |
| [getCharacters](#getcharacters) | Returns all Characters objects that represents a range of characters within the cell text. |
| [setCharacters](#setcharacters) | Sets rich text format of the cell. |
| [getMergedRange](#getmergedrange) | Returns a Range object which represents a merged range. |
| [getHtmlString](#gethtmlstring) | Gets the html string which contains data and some formats in this cell. |
| [toString](#tostring) | Returns a string represents the current Cell object. |
| [toJson](#tojson) | Convert Cell to JSON struct data. |
| [equals](#equals) | Checks whether this object refers to the same cell with another. |
| [hashCode](#hashcode) | Serves as a hash function for a particular type. |
| [getConditionalFormattingResult](#getconditionalformattingresult) | Get the result of the conditional formatting.

Returns null if no conditional formatting is applied to this cell, |
| [getValidation](#getvalidation) | Gets the validation applied to this cell. |
| [getValidationValue](#getvalidationvalue) | Gets the value of validation which applied to this cell. |
| [getTable](#gettable) | Gets the table which contains this cell. |
| [getRichValue](#getrichvalue) |  |
| [calculate](#calculate) | Calculates the formula of the cell. |
| [putValue](#putvalue) | Puts a boolean value into the cell. |
| [getStringValue](#getstringvalue) | Gets the string value by specific formatted strategy. |
| [getWidthOfValue](#getwidthofvalue) | Gets the width of the value in unit of pixels. |
| [getHeightOfValue](#getheightofvalue) | Gets the height of the value in unit of pixels. |
| [getDisplayStyle](#getdisplaystyle) | Gets the display style of the cell. If this cell is also affected by other settings such as conditional formatting, list |
| [getFormatConditions](#getformatconditions) | Gets format conditions which applies to this cell. |
| [getStyle](#getstyle) | Gets the cell style.

To change the style of the cell, please call Cell.SetStyle() method after modifying the returned s |
| [setStyle](#setstyle) | Sets the cell style.

If the border settings are changed, the border of adjust cells will be updated too. |
| [setFormula](#setformula) | Set the formula and the value(calculated result) of the formula. |
| [getFormula](#getformula) | Get the formula of this cell. |
| [setArrayFormula](#setarrayformula) | Sets an array formula to a range of cells.

NOTE: This class is now obsolete. Instead, please use Cell.SetArrayFormula(s |
| [setSharedFormula](#setsharedformula) | Sets a formula to a range of cells.

NOTE: This class is now obsolete. Instead, please use Cell.SetSharedFormula(string, |
| [getPrecedents](#getprecedents) | Gets all references appearing in this cell's formula.

Returns null if this is not a formula cell. All references appear |
| [getDependents](#getdependents) | Get all cells whose formula references to this cell directly.

If one reference containing this cell appears in one cell |
| [getPrecedentsInCalculation](#getprecedentsincalculation) | Gets all precedents(reference to cells in current workbook) used by this cell's formula while calculating it.

This meth |
| [getDependentsInCalculation](#getdependentsincalculation) | Gets all cells whose calculated result depends on this cell.

To use this method, please make sure the workbook has been |
| [getLeafs](#getleafs) | Get all cells which reference to this cell directly and need to be updated when this cell is modified.

NOTE: This class |

### Cell.Worksheet property {#worksheet}

Gets the parent worksheet.

**Type:** Worksheet

### Cell.DateTimeValue property {#datetimevalue}

Gets the DateTime value contained in the cell.

**Type:** DateTime

### Cell.Row property {#row}

Gets row number (zero based) of the cell.

**Type:** Number

### Cell.Column property {#column}

Gets column number (zero based) of the cell.

**Type:** Number

### Cell.IsFormula property {#isformula}

Represents if the specified cell contains formula.

**Type:** boolean

### Cell.HasCustomFunction property {#hascustomfunction}

**Type:** boolean

### Cell.Type property {#type}

Represents cell value type. The value of the property is CellValueType integer constant.

**Type:** Number

### Cell.Name property {#name}

Gets the name of the cell. A cell name includes its column letter and row number. For example, the name of a cell in row 0 and column 0 is A1.

**Type:** String

### Cell.IsErrorValue property {#iserrorvalue}

Checks if the value of this cell is an error. Also applies to formula cell to check whether the calculated result is an error.

**Type:** boolean

### Cell.IsNumericValue property {#isnumericvalue}

Indicates whether the value of this cell is numeric(int, double and datetime) Also applies to formula cell to check the calculated result

**Type:** boolean

### Cell.StringValue property {#stringvalue}

Gets the string value contained in the cell. If the type of this cell is string, then return the string value itself. For other cell types, the formatted string value (formatted with the specified style of this cell) will be returned. The formatted cell value is same with what you can get from excel when copying a cell as text(such as copying cell to text editor or exporting to csv).

**Type:** String

### Cell.StringValueWithoutFormat property {#stringvaluewithoutformat}

Gets cell's value as string without any format. NOTE: This method is now obsolete. Instead, User should get the value object and format it according to the value type and the specific requirement. This property will be removed 12 months later since December 2020. Aspose apologizes for any inconvenience you may have experienced.

**Type:** String

### Cell.NumberCategoryType property {#numbercategorytype}

Represents the category type of this cell's number formatting. The value of the property is NumberCategoryType integer constant. When cell's formatting pattern is combined with conditional formatting patterns, then the returned type is corresponding to the part which is used for current value of this cell. For example, if the formatting pattern for this cell is "#,##0;(#,##0);"-";@", then when cell's value is numeric and not 0, the returned type is NumberCategoryType.NUMBER ; When cell's value is 0 or not numeric value, the returned type is NumberCategoryType.TEXT .

**Type:** Number

### Cell.DisplayStringValue property {#displaystringvalue}

Gets the formatted string value of this cell by cell's display style.

**Type:** String

### Cell.IntValue property {#intvalue}

Gets the integer value contained in the cell.

**Type:** Number

### Cell.DoubleValue property {#doublevalue}

Gets the double value contained in the cell.

**Type:** Number

### Cell.FloatValue property {#floatvalue}

Gets the float value contained in the cell.

**Type:** Number

### Cell.BoolValue property {#boolvalue}

Gets the boolean value contained in the cell.

**Type:** boolean

### Cell.HasCustomStyle property {#hascustomstyle}

Indicates whether this cell has custom style settings(different from the default one inherited from corresponding row, column, or workbook).

**Type:** boolean

### Cell.SharedStyleIndex property {#sharedstyleindex}

Gets cell's shared style index in the style pool.

**Type:** Number

### Cell.Formula property {#formula}

Gets or sets a formula of the Cell . A formula string always begins with an equal sign (=). And please always use comma(,) as parameters delimiter, such as "=SUM(A1, E1, H2)".

**Type:** String

### Cell.FormulaLocal property {#formulalocal}

Get the locale formatted formula of the cell.

**Type:** String

### Cell.R1C1Formula property {#r1c1formula}

Gets or sets a R1C1 formula of the Cell .

**Type:** String

### Cell.ContainsExternalLink property {#containsexternallink}

Indicates whether this cell contains an external link. Only applies when the cell is a formula cell.

**Type:** boolean

### Cell.IsArrayHeader property {#isarrayheader}

Indicates the cell's formula is an array formula and it is the first cell of the array.

**Type:** boolean

### Cell.IsDynamicArrayFormula property {#isdynamicarrayformula}

Indicates whether the cell's formula is dynamic array formula(true) or legacy array formula(false).

**Type:** boolean

### Cell.IsArrayFormula property {#isarrayformula}

Indicates whether the cell formula is an array formula.

**Type:** boolean

### Cell.IsInArray property {#isinarray}

Indicates whether the cell formula is an array formula. NOTE: This class is now obsolete. Instead, please use Cell.IsArrayFormula to check whether the cell formula is an array formula. This property will be removed 12 months later since May 2018. Aspose apologizes for any inconvenience you may have experienced.

**Type:** boolean

### Cell.IsSharedFormula property {#issharedformula}

Indicates whether the cell formula is part of shared formula.

**Type:** boolean

### Cell.IsTableFormula property {#istableformula}

Indicates whether this cell is part of table formula.

**Type:** boolean

### Cell.IsInTable property {#isintable}

Indicates whether this cell is part of table formula. NOTE: This class is now obsolete. Instead, please use Cell.IsTableFormula to check whether the cell formula is part of table formula. This property will be removed 12 months later since May 2018. Aspose apologizes for any inconvenience you may have experienced.

**Type:** boolean

### Cell.Value property {#value}

Gets/sets the value contained in this cell. Possible type: null, Boolean, DateTime, Double, Integer String. For int value, it may be returned as an Integer object or a Double object. And there is no guarantee that the returned value will be kept as the same type of object always.

**Type:** Object

### Cell.IsStyleSet property {#isstyleset}

Indicates if the cell's style is set. If return false, it means this cell has a default cell format.

**Type:** boolean

### Cell.IsMerged property {#ismerged}

Checks if a cell is part of a merged range or not.

**Type:** boolean

### Cell.Comment property {#comment}

Gets the comment of this cell. If there is no comment applies to the cell, returns null.

**Type:** Comment

### Cell.HtmlString property {#htmlstring}

Gets and sets the html string which contains data and some formats in this cell.

**Type:** String

### Cell.IsCheckBoxStyle property {#ischeckboxstyle}

**Type:** boolean

### Cell.EmbeddedImage property {#embeddedimage}

Gets and sets the embeddedn image in the cell.

**Type:** byte[]

### getArrayRange() {#getarrayrange}

Gets the array range if the cell's formula is an array formula.

Only applies when the cell's formula is an array formula

**Returns:** The array range.

### setDynamicArrayFormula(arrayFormula, options, calculateValue) (1 of 3) {#setdynamicarrayformula}

Sets dynamic array formula and make the formula spill into neighboring cells if possible.

the returned range may be not same with the actual one that this dynamic array formula spills into. If there are non-empty cells in the range, the formula will be set for current cell only and marked as "#SPILL!". But for such kind of situation we still return the whole range that this formula should spill into.

| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | the formula expression |
| options | FormulaParseOptions | options to parse formula. "Parse" option will be ignored and the formula will always be parsed immediately |
| calculateValue | boolean | whether calculate this dynamic array formula for those cells in the spilled range. |

**Returns:** the range that the formula should spill into.

---

### setDynamicArrayFormula(arrayFormula, options, values, calculateRange, calculateValue) (2 of 3) {#setdynamicarrayformula-1}

Sets dynamic array formula and make the formula spill into neighboring cells if possible.

the returned range may be not same with the actual one that this dynamic array formula spills into. If there are non-empty cells in the range, the formula will be set for current cell only and marked as "#SPILL!". But for such kind of situation we still return the whole range that this formula should spill into.

| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | the formula expression |
| options | FormulaParseOptions | options to parse formula. "Parse" option will be ignored and the formula will always be parsed immediately |
| values | Object[][] | values(calculated results) for those cells with given dynamic array formula |
| calculateRange | boolean | Whether calculate the spilled range for this dynamic array formula. If the "values" parameter is not null and this flag is false, then the spilled range's height will be values.Length and width will be values[0].Length. |
| calculateValue | boolean | whether calculate this dynamic array formula for those cells in the spilled range when "values" is null or corresponding item in "values" for one cell is null. |

**Returns:** the range that the formula should spill into.

---

### setDynamicArrayFormula(arrayFormula, options, values, calculateRange, calculateValue, copts) (3 of 3) {#setdynamicarrayformula-2}

Sets dynamic array formula and make the formula spill into neighboring cells if possible.

the returned range may be not same with the actual one that this dynamic array formula spills into. If there are non-empty cells in the range, the formula will be set for current cell only and marked as "#SPILL!". But for such kind of situation we still return the whole range that this formula should spill into.

| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | the formula expression |
| options | FormulaParseOptions | options to parse formula. "Parse" option will be ignored and the formula will always be parsed immediately |
| values | Object[][] | values(calculated results) for those cells with given dynamic array formula |
| calculateRange | boolean | Whether calculate the spilled range for this dynamic array formula. If the "values" parameter is not null and this flag is false, then the spilled range's height will be values.Length and width will be values[0].Length. |
| calculateValue | boolean | whether calculate this dynamic array formula for those cells in the spilled range when "values" is null or corresponding item in "values" for one cell is null. |
| copts | CalculationOptions | The options for calculating formula. Commonly, for performance consideration, the CalculationOptions.Recursive property should be false. |

**Returns:** the range that the formula should spill into.

### setTableFormula(rowNumber, columnNumber, rowInputCell, columnInputCell, values) (1 of 4) {#settableformula}

Create two-variable data table for given range starting from this cell.

| Parameter | Type | Description |
| --- | --- | --- |
| rowNumber | Number | Number of rows to populate the formula. |
| columnNumber | Number | Number of columns to populate the formula. |
| rowInputCell | String | the row input cell |
| columnInputCell | String | the column input cell |
| values | Object[][] | values for cells in table formula range |

---

### setTableFormula(rowNumber, columnNumber, inputCell, isRowInput, values) (2 of 4) {#settableformula-1}

Create one-variable data table for given range starting from this cell.

| Parameter | Type | Description |
| --- | --- | --- |
| rowNumber | Number | Number of rows to populate the formula. |
| columnNumber | Number | Number of columns to populate the formula. |
| inputCell | String | the input cell |
| isRowInput | boolean | Indicates whether the input cell is a row input cell(true) or a column input cell(false). |
| values | Object[][] | values for cells in table formula range |

---

### setTableFormula(rowNumber, columnNumber, rowIndexOfRowInputCell, columnIndexOfRowInputCell, rowIndexOfColumnInputCell, columnIndexOfColumnInputCell, values) (3 of 4) {#settableformula-2}

Create two-variable data table for given range starting from this cell.

| Parameter | Type | Description |
| --- | --- | --- |
| rowNumber | Number | Number of rows to populate the formula. |
| columnNumber | Number | Number of columns to populate the formula. |
| rowIndexOfRowInputCell | Number | row index of the row input cell |
| columnIndexOfRowInputCell | Number | column index of the row input cell |
| rowIndexOfColumnInputCell | Number | row index of the column input cell |
| columnIndexOfColumnInputCell | Number | column index of the column input cell |
| values | Object[][] | values for cells in table formula range |

---

### setTableFormula(rowNumber, columnNumber, rowIndexOfInputCell, columnIndexOfInputCell, isRowInput, values) (4 of 4) {#settableformula-3}

Create one-variable data table for given range starting from this cell.

| Parameter | Type | Description |
| --- | --- | --- |
| rowNumber | Number | Number of rows to populate the formula. |
| columnNumber | Number | Number of columns to populate the formula. |
| rowIndexOfInputCell | Number | row index of the input cell |
| columnIndexOfInputCell | Number | column index of the input cell |
| isRowInput | boolean | Indicates whether the input cell is a row input cell(true) or a column input cell(false). |
| values | Object[][] | values for cells in table formula range |

### removeArrayFormula(leaveNormalFormula) {#removearrayformula}

Remove array formula.

| Parameter | Type | Description |
| --- | --- | --- |
| leaveNormalFormula | boolean | True represents converting the array formula to normal formula. |

### copy(cell) {#copy}

Copies data from a source cell.

| Parameter | Type | Description |
| --- | --- | --- |
| cell | Cell | Source Cell object. |

### characters(startIndex, length) {#characters}

Returns a Characters object that represents a range of characters within the cell text.

This method only works on cell with string value.

| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | Number | The index of the start of the character. |
| length | Number | The number of characters. |

**Returns:** Characters object.

**Example:**

```php
$workbook = new cells\Workbook();
$cell = $workbook->getWorksheets()->get(0)->getCells()->get("A1");
$cell->putValue("Helloworld");
$cell->characters(5, 5)->getFont()->setBold(true);
$cell->characters(5, 5)->getFont()->setColor(cells\Color::getBlue());
```

### replace(placeHolder, newValue, options) {#replace}

Replace text of the cell with options.

| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValue | String | String value to replace |
| options | ReplaceOptions | The replace options |

### insertText(index, text) {#inserttext}

Insert some characters to the cell. If the cell is rich formatted, this method could keep the original formatting.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The index. |
| text | String | Inserted text. |

### isRichText() {#isrichtext}

Indicates whether the string value of this cell is a rich formatted text.

### getCharacters() (1 of 2) {#getcharacters}

Returns all Characters objects that represents a range of characters within the cell text.

**Returns:** All Characters objects

---

### getCharacters(flag) (2 of 2) {#getcharacters-1}

Returns all Characters objects that represents a range of characters within the cell text.

| Parameter | Type | Description |
| --- | --- | --- |
| flag | boolean | Indicates whether applying table style to the cell if the cell is in the table. |

**Returns:** All Characters objects

### setCharacters(characters) {#setcharacters}

Sets rich text format of the cell.

| Parameter | Type | Description |
| --- | --- | --- |
| characters | FontSetting[] | All Characters objects. |

### getMergedRange() {#getmergedrange}

Returns a Range object which represents a merged range.

**Returns:** Range object. Null if this cell is not merged.

### getHtmlString(html5) {#gethtmlstring}

Gets the html string which contains data and some formats in this cell.

| Parameter | Type | Description |
| --- | --- | --- |
| html5 | boolean | Indicates whether the value is compatible for html5 |

### toString() {#tostring}

Returns a string represents the current Cell object.

### toJson() {#tojson}

Convert Cell to JSON struct data.

### equals(obj) (1 of 2) {#equals}

Checks whether this object refers to the same cell with another.

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | another object |

**Returns:** true if two objects refers to the same cell.

---

### equals(cell) (2 of 2) {#equals-1}

Checks whether this object refers to the same cell with another cell object.

| Parameter | Type | Description |
| --- | --- | --- |
| cell | Cell | another cell object |

**Returns:** true if two cell objects refers to the same cell.

### hashCode() {#hashcode}

Serves as a hash function for a particular type.

**Returns:** A hash code for current Cell object.

### getConditionalFormattingResult() {#getconditionalformattingresult}

Get the result of the conditional formatting.

Returns null if no conditional formatting is applied to this cell,

### getValidation() {#getvalidation}

Gets the validation applied to this cell.

### getValidationValue() {#getvalidationvalue}

Gets the value of validation which applied to this cell.

### getTable() {#gettable}

Gets the table which contains this cell.

### getRichValue() {#getrichvalue}

### calculate(options) {#calculate}

Calculates the formula of the cell.

| Parameter | Type | Description |
| --- | --- | --- |
| options | CalculationOptions | Options for calculation |

### putValue(boolValue) (1 of 8) {#putvalue}

Puts a boolean value into the cell.

| Parameter | Type | Description |
| --- | --- | --- |
| boolValue | boolean |  |

---

### putValue(intValue) (2 of 8) {#putvalue-1}

Puts an integer value into the cell.

| Parameter | Type | Description |
| --- | --- | --- |
| intValue | Number | Input value |

---

### putValue(doubleValue) (3 of 8) {#putvalue-2}

Puts a double value into the cell.

| Parameter | Type | Description |
| --- | --- | --- |
| doubleValue | Number | Input value |

---

### putValue(stringValue, isConverted, setStyle) (4 of 8) {#putvalue-3}

Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will be reset.

| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | String | Input value |
| isConverted | boolean | True: converted to other data type if appropriate. |
| setStyle | boolean | True: set the number format to cell's style when converting to other data type |

---

### putValue(stringValue, isConverted) (5 of 8) {#putvalue-4}

Puts a string value into the cell and converts the value to other data type if appropriate.

| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | String | Input value |
| isConverted | boolean | True: converted to other data type if appropriate. |

---

### putValue(stringValue) (6 of 8) {#putvalue-5}

Puts a string value into the cell.

| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | String | Input value |

---

### putValue(dateTime) (7 of 8) {#putvalue-6}

Puts a DateTime value into the cell.

Setting a DateTime value for a cell dose not means the cell will be formatted as date time automatically. DateTime value was maintained as numeric value in the data model of both ms excel and Aspose.Cells. Whether the numeric value will be taken as the numeric value itself or date time depends on the number format applied on this cell. If this cell has not been formatted as date time, it will be displayed as a numeric value even though what you input is DateTime.

| Parameter | Type | Description |
| --- | --- | --- |
| dateTime | DateTime | Input value |

---

### putValue(objectValue) (8 of 8) {#putvalue-7}

Puts an object value into the cell.

| Parameter | Type | Description |
| --- | --- | --- |
| objectValue | Object | input value |

### getStringValue(formatStrategy) {#getstringvalue}

Gets the string value by specific formatted strategy.

| Parameter | Type | Description |
| --- | --- | --- |
| formatStrategy | Number | A CellValueFormatStrategy value. The formatted strategy. |

### getWidthOfValue() {#getwidthofvalue}

Gets the width of the value in unit of pixels.

### getHeightOfValue() {#getheightofvalue}

Gets the height of the value in unit of pixels.

### getDisplayStyle() (1 of 3) {#getdisplaystyle}

Gets the display style of the cell. If this cell is also affected by other settings such as conditional formatting, list objects, etc., then the display style may be different from cell.GetStyle().

---

### getDisplayStyle(includeMergedBorders) (2 of 3) {#getdisplaystyle-1}

Gets the display style of the cell. If the cell is conditional formatted, the display style is not same as the cell.GetStyle().

| Parameter | Type | Description |
| --- | --- | --- |
| includeMergedBorders | boolean | Indicates whether checking borders of the merged cells. |

---

### getDisplayStyle(adjacentBorders) (3 of 3) {#getdisplaystyle-2}

### getFormatConditions() {#getformatconditions}

Gets format conditions which applies to this cell.

**Returns:** Returns FormatConditionCollection object

### getStyle() (1 of 2) {#getstyle}

Gets the cell style.

To change the style of the cell, please call Cell.SetStyle() method after modifying the returned style object. This method is same with getStyle(boolean) with true value for the parameter.

**Returns:** Style object.

---

### getStyle(checkBorders) (2 of 2) {#getstyle-1}

If checkBorders is true, check whether other cells' borders will effect the style of this cell.

| Parameter | Type | Description |
| --- | --- | --- |
| checkBorders | boolean | Check other cells' borders |

**Returns:** Style object.

### setStyle(style) (1 of 3) {#setstyle}

Sets the cell style.

If the border settings are changed, the border of adjust cells will be updated too.

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The cell style. |

---

### setStyle(style, explicitFlag) (2 of 3) {#setstyle-1}

Apply the changed property of style to the cell.

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The cell style. |
| explicitFlag | boolean | True, only overwriting formatting which is explicitly set. |

---

### setStyle(style, flag) (3 of 3) {#setstyle-2}

Apply the cell style based on flags.

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The cell style. |
| flag | StyleFlag | The style flag. |

### setFormula(formula, value) (1 of 4) {#setformula}

Set the formula and the value(calculated result) of the formula.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The formula. |
| value | Object | The value(calculated result) of the formula. |

---

### setFormula(formula, options) (2 of 4) {#setformula-1}

---

### setFormula(formula, isR1C1, isLocal, value) (3 of 4) {#setformula-2}

Set the formula and the value of the formula.

NOTE: This class is now obsolete. Instead, please use Cell.SetFormula(string,FormulaParseOptions,object). This property will be removed 12 months later since December 2019. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The formula. |
| isR1C1 | boolean | Whether the formula is R1C1 formula. |
| isLocal | boolean | Whether the formula is locale formatted. |
| value | Object | The value of the formula. |

---

### setFormula(formula, options, value) (4 of 4) {#setformula-3}

Set the formula and the value(calculated result) of the formula.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The formula. |
| options | FormulaParseOptions | Options for parsing the formula. |
| value | Object | The value(calculated result) of the formula. |

### getFormula(isR1C1, isLocal) {#getformula}

Get the formula of this cell.

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns:** the formula of this cell.

### setArrayFormula(arrayFormula, rowNumber, columnNumber, isR1C1, isLocal) (1 of 4) {#setarrayformula}

Sets an array formula to a range of cells.

NOTE: This class is now obsolete. Instead, please use Cell.SetArrayFormula(string,int,int,FormulaParseOptions). This property will be removed 12 months later since December 2019. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | Array formula. |
| rowNumber | Number | Number of rows to populate result of the array formula. |
| columnNumber | Number | Number of columns to populate result of the array formula. |
| isR1C1 | boolean | whether the formula is R1C1 formula |
| isLocal | boolean | whether the formula is locale formatted |

---

### setArrayFormula(arrayFormula, rowNumber, columnNumber) (2 of 4) {#setarrayformula-1}

Sets an array formula(legacy array formula entered via CTRL+SHIFT+ENTER in ms excel) to a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | Array formula. |
| rowNumber | Number | Number of rows to populate result of the array formula. |
| columnNumber | Number | Number of columns to populate result of the array formula. |

---

### setArrayFormula(arrayFormula, rowNumber, columnNumber, options) (3 of 4) {#setarrayformula-2}

Sets an array formula to a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | Array formula. |
| rowNumber | Number | Number of rows to populate result of the array formula. |
| columnNumber | Number | Number of columns to populate result of the array formula. |
| options | FormulaParseOptions | Options for parsing the formula. |

---

### setArrayFormula(arrayFormula, rowNumber, columnNumber, options, values) (4 of 4) {#setarrayformula-3}

Sets an array formula to a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | Array formula. |
| rowNumber | Number | Number of rows to populate result of the array formula. |
| columnNumber | Number | Number of columns to populate result of the array formula. |
| options | FormulaParseOptions | Options for parsing the formula. |
| values | Object[][] | values for those cells with given array formula |

### setSharedFormula(sharedFormula, rowNumber, columnNumber, isR1C1, isLocal) (1 of 4) {#setsharedformula}

Sets a formula to a range of cells.

NOTE: This class is now obsolete. Instead, please use Cell.SetSharedFormula(string,int,int,FormulaParseOptions). This property will be removed 12 months later since December 2019. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| sharedFormula | String | Shared formula. |
| rowNumber | Number | Number of rows to populate the formula. |
| columnNumber | Number | Number of columns to populate the formula. |
| isR1C1 | boolean | whether the formula is R1C1 formula |
| isLocal | boolean | whether the formula is locale formatted |

---

### setSharedFormula(sharedFormula, rowNumber, columnNumber) (2 of 4) {#setsharedformula-1}

Sets shared formulas to a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| sharedFormula | String | Shared formula. |
| rowNumber | Number | Number of rows to populate the formula. |
| columnNumber | Number | Number of columns to populate the formula. |

---

### setSharedFormula(sharedFormula, rowNumber, columnNumber, options) (3 of 4) {#setsharedformula-2}

Sets shared formulas to a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| sharedFormula | String | Shared formula. |
| rowNumber | Number | Number of rows to populate the formula. |
| columnNumber | Number | Number of columns to populate the formula. |
| options | FormulaParseOptions | Options for parsing the formula. |

---

### setSharedFormula(sharedFormula, rowNumber, columnNumber, options, values) (4 of 4) {#setsharedformula-3}

Sets shared formulas to a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| sharedFormula | String | Shared formula. |
| rowNumber | Number | Number of rows to populate the formula. |
| columnNumber | Number | Number of columns to populate the formula. |
| options | FormulaParseOptions | Options for parsing the formula. |
| values | Object[][] | values for those cells with given shared formula |

### getPrecedents() {#getprecedents}

Gets all references appearing in this cell's formula.

Returns null if this is not a formula cell. All references appearing in this cell's formula will be returned no matter they are referenced or not while calculating. For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating, it is still taken as the formula's precedents. To get those references which influence the calculation only, please use getPrecedentsInCalculation() .

**Returns:** Collection of all references appearing in this cell's formula.

**Example:**

```php
$workbook = new cells\Workbook();
$cells = $workbook->getWorksheets()->get(0)->getCells();
$cells->get("A1")->setFormula("= B1 + SUM(B1:B10) + [Book1.xls]Sheet1!A1");
$areas =$cells->get("A1")->getPrecedents();
for ($i = 0; $i < java_values($areas->getCount()); $i++)
{
    $area = $areas->get($i);
    $stringBuilder = "";
    if (java_values($area->isExternalLink()))
    {
        $stringBuilder .= "[";
        $stringBuilder .= $area->getExternalFileName();
        $stringBuilder .= "]";
    }
    $stringBuilder .= $area->getSheetName();
    $stringBuilder .= "!";
    $stringBuilder .= cells\CellsHelper::cellIndexToName($area->getStartRow(), $area->getStartColumn());
    if (java_values($area->isArea()))
    {
        $stringBuilder .= ":";
        $stringBuilder .= cells\CellsHelper::cellIndexToName($area->getEndRow(), $area->getEndColumn());
    }
    echo "Precedent ".$i.": ".$stringBuilder."\n";
}
```

### getDependents(isAll) {#getdependents}

Get all cells whose formula references to this cell directly.

If one reference containing this cell appears in one cell's formula, that cell will be taken as the dependent of this cell, no matter the reference or this cell is used or not while calculating. For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating, this formula is still be taken as A2's dependent. To get those formulas whose calculated results depend on this cell, please use getDependentsInCalculation(boolean) . When tracing dependents for one cell, all formulas in the workbook or worksheet will be analized and checked. So it is a time consumed process. If user need to trace dependents for lots of cells, using this method will cause poor performance. For performance consideration, user should use getDependentsInCalculation(boolean) instead. Or, user may gather precedents map of all cells by getPrecedents() firstly, and then build the dependents map according to the precedents map.

| Parameter | Type | Description |
| --- | --- | --- |
| isAll | boolean | Indicates whether check formulas in other worksheets |

### getPrecedentsInCalculation() {#getprecedentsincalculation}

Gets all precedents(reference to cells in current workbook) used by this cell's formula while calculating it.

This method can only work with the situation that FormulaSettings.EnableCalculationChain is true for the workbook and the workbook has been fully calculated. If this cell is not a formula or it does not reference to any other cells, null will be returned.

**Returns:** Enumerator to enumerate all references(ReferredArea)

### getDependentsInCalculation(recursive) {#getdependentsincalculation}

Gets all cells whose calculated result depends on this cell.

To use this method, please make sure the workbook has been set with true value for FormulaSettings.EnableCalculationChain and has been fully calculated with this setting. If there is no formula reference to this cell, null will be returned.

| Parameter | Type | Description |
| --- | --- | --- |
| recursive | boolean | Whether returns those dependents which do not reference to this cell directly but reference to other leafs of this cell |

**Returns:** Enumerator to enumerate all dependents(Cell objects)

### getLeafs() (1 of 2) {#getleafs}

Get all cells which reference to this cell directly and need to be updated when this cell is modified.

NOTE: This class is now obsolete. Instead, please use Cell.GetDependentsInCalculation(bool) to get all dependents in calculation chain. This property will be removed 12 months later since May 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:** Enumerator to enumerate all dependents(Cell)

---

### getLeafs(recursive) (2 of 2) {#getleafs-1}

Get all cells which will be updated when this cell is modified.

NOTE: This class is now obsolete. Instead, please use Cell.GetDependentsInCalculation(bool) to get all dependents in calculation chain. This property will be removed 12 months later since May 2022. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| recursive | boolean | Whether returns those leafs that do not reference to this cell directly but reference to other leafs of this cell |

**Returns:** Enumerator to enumerate all dependents(Cell)
