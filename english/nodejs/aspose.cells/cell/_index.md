---
title: "Cell"
linktitle: "Cell"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Encapsulates the object that represents a single Workbook cell."
type: docs
weight: 340
url: /nodejs/aspose.cells/cell/
---

## Cell class

Encapsulates the object that represents a single Workbook cell.

## Methods

| Name | Description |
| --- | --- |
| [calculate(options)](#calculate) | Calculates the formula of the cell. |
| [characters(startIndex, length)](#characters) | Returns a Characters object that represents a range of characters within the cell text. This method only works on cell w |
| [containsExternalLink()](#containsexternallink) | Indicates whether this cell contains an external link. Only applies when the cell is a formula cell. |
| [copy(cell)](#copy) | Copies data from a source cell. |
| [equals(obj)](#equals) | Checks whether this object refers to the same cell with another. |
| [equals(cell)](#equals-1) | Checks whether this object refers to the same cell with another cell object. |
| [getArrayRange()](#getarrayrange) | Gets the array range if the cell's formula is an array formula. Only applies when the cell's formula is an array formula |
| [getBoolValue()](#getboolvalue) | Gets the boolean value contained in the cell. |
| [getCharacters()](#getcharacters) | Returns all Characters objects that represents a range of characters within the cell text. |
| [getCharacters(flag)](#getcharacters-1) | Returns all Characters objects that represents a range of characters within the cell text. |
| [getColumn()](#getcolumn) | Gets column number (zero based) of the cell. |
| [getComment()](#getcomment) | Gets the comment of this cell. If there is no comment applies to the cell, returns null. |
| [getConditionalFormattingResult()](#getconditionalformattingresult) | Get the result of the conditional formatting. Returns null if no conditional formatting is applied to this cell, |
| [getDateTimeValue()](#getdatetimevalue) | Gets the DateTime value contained in the cell. |
| [getDependents(isAll)](#getdependents) | Get all cells whose formula references to this cell directly. If one reference containing this cell appears in one cell' |
| [getDependentsInCalculation(recursive)](#getdependentsincalculation) | Gets all cells whose calculated result depends on this cell. To use this method, please make sure the workbook has been  |
| [getDisplayStringValue()](#getdisplaystringvalue) | Gets the formatted string value of this cell by cell's display style. |
| [getDisplayStyle()](#getdisplaystyle) | Gets the display style of the cell. If this cell is also affected by other settings such as conditional formatting, list |
| [getDisplayStyle(includeMergedBorders)](#getdisplaystyle-1) | Gets the display style of the cell. If the cell is conditional formatted, the display style is not same as the cell.GetS |
| [getDisplayStyle()](#getdisplaystyle-2) |  |
| [getDoubleValue()](#getdoublevalue) | Gets the double value contained in the cell. |
| [getEmbeddedImage()](#getembeddedimage) | Gets and sets the embeddedn image in the cell. |
| [getFloatValue()](#getfloatvalue) | Gets the float value contained in the cell. |
| [getFormatConditions()](#getformatconditions) | Gets format conditions which applies to this cell. |
| [getFormula()](#getformula) | Gets or sets a formula of the Cell. A formula string always begins with an equal sign (=). And please always use comma(, |
| [getFormula(isR1C1, isLocal)](#getformula-1) | Get the formula of this cell. |
| [getFormulaLocal()](#getformulalocal) | Get the locale formatted formula of the cell. |
| [getHeightOfValue()](#getheightofvalue) | Gets the height of the value in unit of pixels. |
| [getHtmlString()](#gethtmlstring) | Gets and sets the html string which contains data and some formats in this cell. |
| [getHtmlString(html5)](#gethtmlstring-1) | Gets the html string which contains data and some formats in this cell. |
| [getIntValue()](#getintvalue) | Gets the integer value contained in the cell. |
| [getLeafs()](#getleafs) | Get all cells which reference to this cell directly and need to be updated when this cell is modified. NOTE: This class  |
| [getLeafs(recursive)](#getleafs-1) | Get all cells which will be updated when this cell is modified. NOTE: This class is now obsolete. Instead, please use Ce |
| [getMergedRange()](#getmergedrange) | Returns a Range object which represents a merged range. |
| [getName()](#getname) | Gets the name of the cell. A cell name includes its column letter and row number. For example, the name of a cell in row |
| [getNumberCategoryType()](#getnumbercategorytype) | Represents the category type of this cell's number formatting. The value of the property is NumberCategoryType integer c |
| [getPrecedents()](#getprecedents) | Gets all references appearing in this cell's formula. Returns null if this is not a formula cell.All references appearin |
| [getPrecedentsInCalculation()](#getprecedentsincalculation) | Gets all precedents(reference to cells in current workbook) used by this cell's formula while calculating it. This metho |
| [getR1C1Formula()](#getr1c1formula) | Gets or sets a R1C1 formula of the Cell. |
| [getRichValue()](#getrichvalue) |  |
| [getRow()](#getrow) | Gets row number (zero based) of the cell. Cell row number |
| [getSharedStyleIndex()](#getsharedstyleindex) | Gets cell's shared style index in the style pool. |
| [getStringValue()](#getstringvalue) | Gets the string value contained in the cell. If the type of this cell is string, then return the string value itself. Fo |
| [getStringValue(formatStrategy)](#getstringvalue-1) | Gets the string value by specific formatted strategy. |
| [getStringValueWithoutFormat()](#getstringvaluewithoutformat) | Gets cell's value as string without any format. NOTE: This method is now obsolete. Instead, User should get the value ob |
| [getStyle()](#getstyle) | Gets the cell style. To change the style of the cell, please call Cell.SetStyle() method after modifying the returned st |
| [getStyle(checkBorders)](#getstyle-1) | If checkBorders is true, check whether other cells' borders will effect the style of this cell. |
| [getTable()](#gettable) | Gets the table which contains this cell. |
| [getType()](#gettype) | Represents cell value type. The value of the property is CellValueType integer constant. |
| [getValidation()](#getvalidation) | Gets the validation applied to this cell. |
| [getValidationValue()](#getvalidationvalue) | Gets the value of validation which applied to this cell. |
| [getValue()](#getvalue) | Gets/sets the value contained in this cell. Possible type: null,Boolean,DateTime,Double,IntegerString. For int value, it |
| [getWidthOfValue()](#getwidthofvalue) | Gets the width of the value in unit of pixels. |
| [getWorksheet()](#getworksheet) | Gets the parent worksheet. |
| [hasCustomFunction()](#hascustomfunction) |  |
| [hasCustomStyle()](#hascustomstyle) | Indicates whether this cell has custom style settings(different from the default one inherited from corresponding row, c |
| [hashCode()](#hashcode) | Serves as a hash function for a particular type. |
| [insertText(index, text)](#inserttext) | Insert some characters to the cell. If the cell is rich formatted, this method could keep the original formatting. |
| [isArrayFormula()](#isarrayformula) | Indicates whether the cell formula is an array formula. |
| [isArrayHeader()](#isarrayheader) | Indicates the cell's formula is an array formula and it is the first cell of the array. |
| [isCheckBoxStyle()](#ischeckboxstyle) |  |
| [isDynamicArrayFormula()](#isdynamicarrayformula) | Indicates whether the cell's formula is dynamic array formula(true) or legacy array formula(false). |
| [isErrorValue()](#iserrorvalue) | Checks if the value of this cell is an error. Also applies to formula cell to check whether the calculated result is an  |
| [isFormula()](#isformula) | Represents if the specified cell contains formula. |
| [isInArray()](#isinarray) | Indicates whether the cell formula is an array formula. NOTE: This class is now obsolete. Instead, please use Cell.IsArr |
| [isInTable()](#isintable) | Indicates whether this cell is part of table formula. NOTE: This class is now obsolete. Instead, please use Cell.IsTable |
| [isMerged()](#ismerged) | Checks if a cell is part of a merged range or not. |
| [isNumericValue()](#isnumericvalue) | Indicates whether the value of this cell is numeric(int, double and datetime) Also applies to formula cell to check the  |
| [isRichText()](#isrichtext) | Indicates whether the string value of this cell is a rich formatted text. |
| [isSharedFormula()](#issharedformula) | Indicates whether the cell formula is part of shared formula. |
| [isStyleSet()](#isstyleset) | Indicates if the cell's style is set. If return false, it means this cell has a default cell format. |
| [isTableFormula()](#istableformula) | Indicates whether this cell is part of table formula. |
| [putValue(boolValue)](#putvalue) | Puts a boolean value into the cell. |
| [putValue(intValue)](#putvalue-1) | Puts an integer value into the cell. |
| [putValue(doubleValue)](#putvalue-2) | Puts a double value into the cell. |
| [putValue(stringValue, isConverted, setStyle)](#putvalue-3) | Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will  |
| [putValue(stringValue, isConverted)](#putvalue-4) | Puts a string value into the cell and converts the value to other data type if appropriate. |
| [putValue(stringValue)](#putvalue-5) | Puts a string value into the cell. |
| [putValue(dateTime)](#putvalue-6) | Puts a DateTime value into the cell. Setting a DateTime value for a cell dose not means the cell will be formatted as da |
| [putValue(objectValue)](#putvalue-7) | Puts an object value into the cell. |
| [removeArrayFormula(leaveNormalFormula)](#removearrayformula) | Remove array formula. |
| [replace(placeHolder, newValue, options)](#replace) | Replace text of the cell with options. |
| [setArrayFormula(arrayFormula, rowNumber, columnNumber, isR1C1, isLocal)](#setarrayformula) | Sets an array formula to a range of cells. NOTE: This class is now obsolete. Instead, please use Cell.SetArrayFormula(st |
| [setArrayFormula(arrayFormula, rowNumber, columnNumber)](#setarrayformula-1) | Sets an array formula(legacy array formula entered via CTRL+SHIFT+ENTER in ms excel) to a range of cells. |
| [setArrayFormula(arrayFormula, rowNumber, columnNumber, options)](#setarrayformula-2) | Sets an array formula to a range of cells. |
| [setArrayFormula(arrayFormula, rowNumber, columnNumber, options, values)](#setarrayformula-3) | Sets an array formula to a range of cells. |
| [setCharacters(characters)](#setcharacters) | Sets rich text format of the cell. |
| [setCheckBoxStyle()](#setcheckboxstyle) |  |
| [setDynamicArrayFormula(arrayFormula, options, calculateValue)](#setdynamicarrayformula) | Sets dynamic array formula and make the formula spill into neighboring cells if possible. |
| [setDynamicArrayFormula(arrayFormula, options, values, calculateRange, calculateValue)](#setdynamicarrayformula-1) | Sets dynamic array formula and make the formula spill into neighboring cells if possible. |
| [setDynamicArrayFormula(arrayFormula, options, values, calculateRange, calculateValue, copts)](#setdynamicarrayformula-2) | Sets dynamic array formula and make the formula spill into neighboring cells if possible. |
| [setEmbeddedImage()](#setembeddedimage) | Gets and sets the embeddedn image in the cell. |
| [setFormula()](#setformula) | Gets or sets a formula of the Cell. A formula string always begins with an equal sign (=). And please always use comma(, |
| [setFormula(formula, value)](#setformula-1) | Set the formula and the value(calculated result) of the formula. |
| [setFormula()](#setformula-2) |  |
| [setFormula(formula, isR1C1, isLocal, value)](#setformula-3) | Set the formula and the value of the formula. NOTE: This class is now obsolete. Instead, please use Cell.SetFormula(stri |
| [setFormula(formula, options, value)](#setformula-4) | Set the formula and the value(calculated result) of the formula. |
| [setFormulaLocal()](#setformulalocal) | Get the locale formatted formula of the cell. |
| [setHtmlString()](#sethtmlstring) | Gets and sets the html string which contains data and some formats in this cell. |
| [setR1C1Formula()](#setr1c1formula) | Gets or sets a R1C1 formula of the Cell. |
| [setSharedFormula(sharedFormula, rowNumber, columnNumber, isR1C1, isLocal)](#setsharedformula) | Sets a formula to a range of cells. NOTE: This class is now obsolete. Instead, please use Cell.SetSharedFormula(string,i |
| [setSharedFormula(sharedFormula, rowNumber, columnNumber)](#setsharedformula-1) | Sets shared formulas to a range of cells. |
| [setSharedFormula(sharedFormula, rowNumber, columnNumber, options)](#setsharedformula-2) | Sets shared formulas to a range of cells. |
| [setSharedFormula(sharedFormula, rowNumber, columnNumber, options, values)](#setsharedformula-3) | Sets shared formulas to a range of cells. |
| [setStyle(style)](#setstyle) | Sets the cell style. If the border settings are changed, the border of adjust cells will be updated too. |
| [setStyle(style, explicitFlag)](#setstyle-1) | Apply the changed property of style to the cell. |
| [setStyle(style, flag)](#setstyle-2) | Apply the cell style based on flags. |
| [setTableFormula(rowNumber, columnNumber, rowInputCell, columnInputCell, values)](#settableformula) | Create two-variable data table for given range starting from this cell. |
| [setTableFormula(rowNumber, columnNumber, inputCell, isRowInput, values)](#settableformula-1) | Create one-variable data table for given range starting from this cell. |
| [setTableFormula(rowNumber, columnNumber, rowIndexOfRowInputCell, columnIndexOfRowInputCell, rowIndexOfColumnInputCell, columnIndexOfColumnInputCell, values)](#settableformula-2) | Create two-variable data table for given range starting from this cell. |
| [setTableFormula(rowNumber, columnNumber, rowIndexOfInputCell, columnIndexOfInputCell, isRowInput, values)](#settableformula-3) | Create one-variable data table for given range starting from this cell. |
| [setValue()](#setvalue) | Gets/sets the value contained in this cell. Possible type: null,Boolean,DateTime,Double,IntegerString. For int value, it |
| [toJson()](#tojson) | Convert Cell to JSON struct data. |
| [toString()](#tostring) | Returns a string represents the current Cell object. |

### calculate(options) {#calculate}

Calculates the formula of the cell.

| Parameter | Type | Description |
| --- | --- | --- |
| options | CalculationOptions | Options for calculation |

### characters(startIndex, length) {#characters}

Returns a Characters object that represents a range of characters within the cell text. This method only works on cell with string value.

| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | Number | The index of the start of the character. |
| length | Number | The number of characters. |

**Returns:** FontSetting — `FontSetting` Characters object.

**Example:**

```js
excel.getWorksheets().get(0).getCells().get("A1").putValue("Helloworld");
excel.getWorksheets().get(0).getCells().get("A1").characters(5, 5).getFont().setBold(true);
excel.getWorksheets().get(0).getCells().get("A1").characters(5, 5).getFont().setColor(aspose.cells.Color.getBlue());
```

### containsExternalLink() {#containsexternallink}

Indicates whether this cell contains an external link. Only applies when the cell is a formula cell.

### copy(cell) {#copy}

Copies data from a source cell.

| Parameter | Type | Description |
| --- | --- | --- |
| cell | Cell | Source |

### equals(obj) {#equals}

Checks whether this object refers to the same cell with another.

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | another object |

**Returns:** boolean — `boolean` true if two objects refers to the same cell.

### equals(cell) {#equals-1}

Checks whether this object refers to the same cell with another cell object.

| Parameter | Type | Description |
| --- | --- | --- |
| cell | Cell | another cell object |

**Returns:** boolean — `boolean` true if two cell objects refers to the same cell.

### getArrayRange() {#getarrayrange}

Gets the array range if the cell's formula is an array formula. Only applies when the cell's formula is an array formula@return {CellArea} The array range.

### getBoolValue() {#getboolvalue}

Gets the boolean value contained in the cell.

### getCharacters() {#getcharacters}

Returns all Characters objects that represents a range of characters within the cell text.

**Returns:** Array ofFontSetting — `Array ofFontSetting` All Characters objects

### getCharacters(flag) {#getcharacters-1}

Returns all Characters objects that represents a range of characters within the cell text.

| Parameter | Type | Description |
| --- | --- | --- |
| flag | boolean | Indicates whether applying table style to the cell if the cell is in the table. |

**Returns:** Array ofFontSetting — `Array ofFontSetting` All Characters objects

### getColumn() {#getcolumn}

Gets column number (zero based) of the cell.

### getComment() {#getcomment}

Gets the comment of this cell. If there is no comment applies to the cell, returns null.

### getConditionalFormattingResult() {#getconditionalformattingresult}

Get the result of the conditional formatting. Returns null if no conditional formatting is applied to this cell,

### getDateTimeValue() {#getdatetimevalue}

Gets the DateTime value contained in the cell.

### getDependents(isAll) {#getdependents}

Get all cells whose formula references to this cell directly. If one reference containing this cell appears in one cell's formula, that cell will be taken as the dependent of this cell, no matter the reference or this cell is used or not while calculating. For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating, this formula is still be taken as A2's dependent. To get those formulas whose calculated results depend on this cell, please use getDependentsInCalculation(boolean).When tracing dependents for one cell, all formulas in the workbook or worksheet will be analized and checked. So it is a time consumed process. If user need to trace dependents for lots of cells, using this method will cause poor performance. For performance consideration, user should use getDependentsInCalculation(boolean) instead. Or, user may gather precedents map of all cells by getPrecedents() firstly, and then build the dependents map according to the precedents map.

| Parameter | Type | Description |
| --- | --- | --- |
| isAll | boolean | Indicates whether check formulas in other worksheets |

### getDependentsInCalculation(recursive) {#getdependentsincalculation}

Gets all cells whose calculated result depends on this cell. To use this method, please make sure the workbook has been set with true value for FormulaSettings.EnableCalculationChain and has been fully calculated with this setting. If there is no formula reference to this cell, null will be returned.

| Parameter | Type | Description |
| --- | --- | --- |
| recursive | boolean | Whether returns those dependents which do not reference to this cell directly but reference to other leafs of this cell |

**Returns:** Iterator — `Iterator` Enumerator to enumerate all dependents(Cell objects)

### getDisplayStringValue() {#getdisplaystringvalue}

Gets the formatted string value of this cell by cell's display style.

### getDisplayStyle() {#getdisplaystyle}

Gets the display style of the cell. If this cell is also affected by other settings such as conditional formatting, list objects, etc., then the display style may be different from cell.GetStyle().

### getDisplayStyle(includeMergedBorders) {#getdisplaystyle-1}

Gets the display style of the cell. If the cell is conditional formatted, the display style is not same as the cell.GetStyle().

| Parameter | Type | Description |
| --- | --- | --- |
| includeMergedBorders | boolean | Indicates whether checking borders of the merged cells. |

### getDisplayStyle() {#getdisplaystyle-2}

### getDoubleValue() {#getdoublevalue}

Gets the double value contained in the cell.

### getEmbeddedImage() {#getembeddedimage}

Gets and sets the embeddedn image in the cell.

### getFloatValue() {#getfloatvalue}

Gets the float value contained in the cell.

### getFormatConditions() {#getformatconditions}

Gets format conditions which applies to this cell.

**Returns:** Array ofFormatConditionCollection — `Array ofFormatConditionCollection` Returns FormatConditionCollection object

### getFormula() {#getformula}

Gets or sets a formula of the Cell. A formula string always begins with an equal sign (=). And please always use comma(,) as parameters delimiter, such as "=SUM(A1, E1, H2)".

**Example:**

```js
var excel = new aspose.cells.Workbook();
var cells = excel.getWorksheets().get(0).getCells();
cells.get("B6").setFormula("=SUM(B2:B5, E1) + sheet2!A1");
```

### getFormula(isR1C1, isLocal) {#getformula-1}

Get the formula of this cell.

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns:** String — `String` the formula of this cell.

### getFormulaLocal() {#getformulalocal}

Get the locale formatted formula of the cell.

### getHeightOfValue() {#getheightofvalue}

Gets the height of the value in unit of pixels.

**Returns:** Number — `Number`

### getHtmlString() {#gethtmlstring}

Gets and sets the html string which contains data and some formats in this cell.

### getHtmlString(html5) {#gethtmlstring-1}

Gets the html string which contains data and some formats in this cell.

| Parameter | Type | Description |
| --- | --- | --- |
| html5 | boolean | Indicates whether the value is compatible for html5 |

**Returns:** String — `String`

### getIntValue() {#getintvalue}

Gets the integer value contained in the cell.

### getLeafs() {#getleafs}

Get all cells which reference to this cell directly and need to be updated when this cell is modified. NOTE: This class is now obsolete. Instead, please use Cell.GetDependentsInCalculation(bool) to get all dependents in calculation chain. This property will be removed 12 months later since May 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:** Iterator — `Iterator` Enumerator to enumerate all dependents(Cell)

### getLeafs(recursive) {#getleafs-1}

Get all cells which will be updated when this cell is modified. NOTE: This class is now obsolete. Instead, please use Cell.GetDependentsInCalculation(bool) to get all dependents in calculation chain. This property will be removed 12 months later since May 2022. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| recursive | boolean | Whether returns those leafs that do not reference to this cell directly but reference to other leafs of this cell |

**Returns:** Iterator — `Iterator` Enumerator to enumerate all dependents(Cell)

### getMergedRange() {#getmergedrange}

Returns a Range object which represents a merged range.

**Returns:** Range — `Range` Range object. Null if this cell is not merged.

### getName() {#getname}

Gets the name of the cell. A cell name includes its column letter and row number. For example, the name of a cell in row 0 and column 0 is A1.

### getNumberCategoryType() {#getnumbercategorytype}

Represents the category type of this cell's number formatting. The value of the property is NumberCategoryType integer constant.When cell's formatting pattern is combined with conditional formatting patterns, then the returned type is corresponding to the part which is used for current value of this cell. For example, if the formatting pattern for this cell is "#,##0;(#,##0);"-";@", then when cell's value is numeric and not 0, the returned type is NumberCategoryType.NUMBER; When cell's value is 0 or not numeric value, the returned type is NumberCategoryType.TEXT.

### getPrecedents() {#getprecedents}

Gets all references appearing in this cell's formula. Returns null if this is not a formula cell.All references appearing in this cell's formula will be returned no matter they are referenced or not while calculating. For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating, it is still taken as the formula's precedents.To get those references which influence the calculation only, please use getPrecedentsInCalculation().@return {ReferredAreaCollection} Collection of all references appearing in this cell's formula.

**Example:**

```js
var workbook = new aspose.cells.Workbook();
var cells = workbook.getWorksheets().get(0).getCells();
cells.get("A1").setFormula("= B1 + SUM(B1:B10) + [Book1.xls]Sheet1!A1");
var areas = cells.get("A1").getPrecedents();
for (var i = 0; i < areas.getCount(); i++)
{
var area = areas.get(i);
var stringBuilder = "";
if (area.isExternalLink())
{
stringBuilder += "[";
stringBuilder += area.getExternalFileName();
stringBuilder += "]";
}
stringBuilder += area.getSheetName();
stringBuilder += "!";
stringBuilder += aspose.cells.CellsHelper.cellIndexToName(area.getStartRow(), area.getStartColumn());
if (area.isArea())
{
stringBuilder += ":";
stringBuilder += aspose.cells.CellsHelper.cellIndexToName(area.getEndRow(), area.getEndColumn());
}
console.log(stringBuilder);
}
workbook.save("Book2.xls");
```

### getPrecedentsInCalculation() {#getprecedentsincalculation}

Gets all precedents(reference to cells in current workbook) used by this cell's formula while calculating it. This method can only work with the situation that FormulaSettings.EnableCalculationChain is true for the workbook and the workbook has been fully calculated. If this cell is not a formula or it does not reference to any other cells, null will be returned.

**Returns:** Iterator — `Iterator` Enumerator to enumerate all references(ReferredArea)

### getR1C1Formula() {#getr1c1formula}

Gets or sets a R1C1 formula of the Cell.

### getRichValue() {#getrichvalue}

### getRow() {#getrow}

Gets row number (zero based) of the cell. Cell row number

### getSharedStyleIndex() {#getsharedstyleindex}

Gets cell's shared style index in the style pool.

### getStringValue() {#getstringvalue}

Gets the string value contained in the cell. If the type of this cell is string, then return the string value itself. For other cell types, the formatted string value (formatted with the specified style of this cell) will be returned. The formatted cell value is same with what you can get from excel when copying a cell as text(such as copying cell to text editor or exporting to csv).

### getStringValue(formatStrategy) {#getstringvalue-1}

Gets the string value by specific formatted strategy.

| Parameter | Type | Description |
| --- | --- | --- |
| formatStrategy | Number | CellValueFormatStrategy |

**Returns:** String — `String`

### getStringValueWithoutFormat() {#getstringvaluewithoutformat}

Gets cell's value as string without any format. NOTE: This method is now obsolete. Instead, User should get the value object and format it according to the value type and the specific requirement. This property will be removed 12 months later since December 2020. Aspose apologizes for any inconvenience you may have experienced.

### getStyle() {#getstyle}

Gets the cell style. To change the style of the cell, please call Cell.SetStyle() method after modifying the returned style object. This method is same with getStyle(boolean) with true value for the parameter.

**Returns:** Style — `Style` Style object.

### getStyle(checkBorders) {#getstyle-1}

If checkBorders is true, check whether other cells' borders will effect the style of this cell.

| Parameter | Type | Description |
| --- | --- | --- |
| checkBorders | boolean | Check other cells' borders |

**Returns:** Style — `Style` Style object.

### getTable() {#gettable}

Gets the table which contains this cell.

**Returns:** ListObject — `ListObject`

### getType() {#gettype}

Represents cell value type. The value of the property is CellValueType integer constant.

### getValidation() {#getvalidation}

Gets the validation applied to this cell.

**Returns:** Validation — `Validation`

### getValidationValue() {#getvalidationvalue}

Gets the value of validation which applied to this cell.

**Returns:** boolean — `boolean`

### getValue() {#getvalue}

Gets/sets the value contained in this cell. Possible type: null,Boolean,DateTime,Double,IntegerString. For int value, it may be returned as an Integer object or a Double object. And there is no guarantee that the returned value will be kept as the same type of object always.

### getWidthOfValue() {#getwidthofvalue}

Gets the width of the value in unit of pixels.

**Returns:** Number — `Number`

### getWorksheet() {#getworksheet}

Gets the parent worksheet.

### hasCustomFunction() {#hascustomfunction}

### hasCustomStyle() {#hascustomstyle}

Indicates whether this cell has custom style settings(different from the default one inherited from corresponding row, column, or workbook).

### hashCode() {#hashcode}

Serves as a hash function for a particular type.

**Returns:** Number — `Number` A hash code for current Cell object.

### insertText(index, text) {#inserttext}

Insert some characters to the cell. If the cell is rich formatted, this method could keep the original formatting.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The index. |
| text | String | Inserted text. |

### isArrayFormula() {#isarrayformula}

Indicates whether the cell formula is an array formula.

### isArrayHeader() {#isarrayheader}

Indicates the cell's formula is an array formula and it is the first cell of the array.

### isCheckBoxStyle() {#ischeckboxstyle}

### isDynamicArrayFormula() {#isdynamicarrayformula}

Indicates whether the cell's formula is dynamic array formula(true) or legacy array formula(false).

### isErrorValue() {#iserrorvalue}

Checks if the value of this cell is an error. Also applies to formula cell to check whether the calculated result is an error.

### isFormula() {#isformula}

Represents if the specified cell contains formula.

### isInArray() {#isinarray}

Indicates whether the cell formula is an array formula. NOTE: This class is now obsolete. Instead, please use Cell.IsArrayFormula to check whether the cell formula is an array formula. This property will be removed 12 months later since May 2018. Aspose apologizes for any inconvenience you may have experienced.

### isInTable() {#isintable}

Indicates whether this cell is part of table formula. NOTE: This class is now obsolete. Instead, please use Cell.IsTableFormula to check whether the cell formula is part of table formula. This property will be removed 12 months later since May 2018. Aspose apologizes for any inconvenience you may have experienced.

### isMerged() {#ismerged}

Checks if a cell is part of a merged range or not.

### isNumericValue() {#isnumericvalue}

Indicates whether the value of this cell is numeric(int, double and datetime) Also applies to formula cell to check the calculated result

### isRichText() {#isrichtext}

Indicates whether the string value of this cell is a rich formatted text.

### isSharedFormula() {#issharedformula}

Indicates whether the cell formula is part of shared formula.

### isStyleSet() {#isstyleset}

Indicates if the cell's style is set. If return false, it means this cell has a default cell format.

### isTableFormula() {#istableformula}

Indicates whether this cell is part of table formula.

### putValue(boolValue) {#putvalue}

Puts a boolean value into the cell.

| Parameter | Type | Description |
| --- | --- | --- |
| boolValue | boolean |  |

### putValue(intValue) {#putvalue-1}

Puts an integer value into the cell.

| Parameter | Type | Description |
| --- | --- | --- |
| intValue | Number | Input value |

### putValue(doubleValue) {#putvalue-2}

Puts a double value into the cell.

| Parameter | Type | Description |
| --- | --- | --- |
| doubleValue | Number | Input value |

### putValue(stringValue, isConverted, setStyle) {#putvalue-3}

Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will be reset.

| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | String | Input value |
| isConverted | boolean | True: converted to other data type if appropriate. |
| setStyle | boolean | True: set the number format to cell's style when converting to other data type |

### putValue(stringValue, isConverted) {#putvalue-4}

Puts a string value into the cell and converts the value to other data type if appropriate.

| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | String | Input value |
| isConverted | boolean | True: converted to other data type if appropriate. |

### putValue(stringValue) {#putvalue-5}

Puts a string value into the cell.

| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | String | Input value |

### putValue(dateTime) {#putvalue-6}

Puts a DateTime value into the cell. Setting a DateTime value for a cell dose not means the cell will be formatted as date time automatically. DateTime value was maintained as numeric value in the data model of both ms excel and Aspose.Cells. Whether the numeric value will be taken as the numeric value itself or date time depends on the number format applied on this cell. If this cell has not been formatted as date time, it will be displayed as a numeric value even though what you input is DateTime.

| Parameter | Type | Description |
| --- | --- | --- |
| dateTime | DateTime | Input value |

### putValue(objectValue) {#putvalue-7}

Puts an object value into the cell.

| Parameter | Type | Description |
| --- | --- | --- |
| objectValue | Object | input value |

### removeArrayFormula(leaveNormalFormula) {#removearrayformula}

Remove array formula.

| Parameter | Type | Description |
| --- | --- | --- |
| leaveNormalFormula | boolean | True represents converting the array formula to normal formula. |

### replace(placeHolder, newValue, options) {#replace}

Replace text of the cell with options.

| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValue | String | String value to replace |
| options | ReplaceOptions | The replace options |

### setArrayFormula(arrayFormula, rowNumber, columnNumber, isR1C1, isLocal) {#setarrayformula}

Sets an array formula to a range of cells. NOTE: This class is now obsolete. Instead, please use Cell.SetArrayFormula(string,int,int,FormulaParseOptions). This property will be removed 12 months later since December 2019. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | Array formula. |
| rowNumber | Number | Number of rows to populate result of the array formula. |
| columnNumber | Number | Number of columns to populate result of the array formula. |
| isR1C1 | boolean | whether the formula is R1C1 formula |
| isLocal | boolean | whether the formula is locale formatted |

### setArrayFormula(arrayFormula, rowNumber, columnNumber) {#setarrayformula-1}

Sets an array formula(legacy array formula entered via CTRL+SHIFT+ENTER in ms excel) to a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | Array formula. |
| rowNumber | Number | Number of rows to populate result of the array formula. |
| columnNumber | Number | Number of columns to populate result of the array formula. |

### setArrayFormula(arrayFormula, rowNumber, columnNumber, options) {#setarrayformula-2}

Sets an array formula to a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | Array formula. |
| rowNumber | Number | Number of rows to populate result of the array formula. |
| columnNumber | Number | Number of columns to populate result of the array formula. |
| options | FormulaParseOptions | Options for parsing the formula. |

### setArrayFormula(arrayFormula, rowNumber, columnNumber, options, values) {#setarrayformula-3}

Sets an array formula to a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | Array formula. |
| rowNumber | Number | Number of rows to populate result of the array formula. |
| columnNumber | Number | Number of columns to populate result of the array formula. |
| options | FormulaParseOptions | Options for parsing the formula. |
| values | Array of Array of Object | values for those cells with given array formula |

### setCharacters(characters) {#setcharacters}

Sets rich text format of the cell.

| Parameter | Type | Description |
| --- | --- | --- |
| characters | Array ofFontSetting | All Characters objects. |

### setCheckBoxStyle() {#setcheckboxstyle}

### setDynamicArrayFormula(arrayFormula, options, calculateValue) {#setdynamicarrayformula}

Sets dynamic array formula and make the formula spill into neighboring cells if possible.

| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | the formula expression |
| options | FormulaParseOptions | options to parse formula. "Parse" option will be ignored and the formula will always be parsed immediately |
| calculateValue | boolean | whether calculate this dynamic array formula for those cells in the spilled range. |

**Returns:** CellArea — `CellArea` the range that the formula should spill into.

### setDynamicArrayFormula(arrayFormula, options, values, calculateRange, calculateValue) {#setdynamicarrayformula-1}

Sets dynamic array formula and make the formula spill into neighboring cells if possible.

| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | the formula expression |
| options | FormulaParseOptions | options to parse formula. "Parse" option will be ignored and the formula will always be parsed immediately |
| values | Array of Array of Object | values(calculated results) for those cells with given dynamic array formula |
| calculateRange | boolean | Whether calculate the spilled range for this dynamic array formula. If the "values" parameter is not null and this flag is false, then the spilled range's height will be values.Length and width will be values[0].Length. |
| calculateValue | boolean | whether calculate this dynamic array formula for those cells in the spilled range when "values" is null or corresponding item in "values" for one cell is null. |

**Returns:** CellArea — `CellArea` the range that the formula should spill into.

### setDynamicArrayFormula(arrayFormula, options, values, calculateRange, calculateValue, copts) {#setdynamicarrayformula-2}

Sets dynamic array formula and make the formula spill into neighboring cells if possible.

| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | the formula expression |
| options | FormulaParseOptions | options to parse formula. "Parse" option will be ignored and the formula will always be parsed immediately |
| values | Array of Array of Object | values(calculated results) for those cells with given dynamic array formula |
| calculateRange | boolean | Whether calculate the spilled range for this dynamic array formula. If the "values" parameter is not null and this flag is false, then the spilled range's height will be values.Length and width will be values[0].Length. |
| calculateValue | boolean | whether calculate this dynamic array formula for those cells in the spilled range when "values" is null or corresponding item in "values" for one cell is null. |
| copts | CalculationOptions | The options for calculating formula. Commonly, for performance consideration, the |

**Returns:** CellArea — `CellArea` the range that the formula should spill into.

### setEmbeddedImage() {#setembeddedimage}

Gets and sets the embeddedn image in the cell.

### setFormula() {#setformula}

Gets or sets a formula of the Cell. A formula string always begins with an equal sign (=). And please always use comma(,) as parameters delimiter, such as "=SUM(A1, E1, H2)".

**Example:**

```js
var excel = new aspose.cells.Workbook();
var cells = excel.getWorksheets().get(0).getCells();
cells.get("B6").setFormula("=SUM(B2:B5, E1) + sheet2!A1");
```

### setFormula(formula, value) {#setformula-1}

Set the formula and the value(calculated result) of the formula.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The formula. |
| value | Object | The value(calculated result) of the formula. |

### setFormula() {#setformula-2}

### setFormula(formula, isR1C1, isLocal, value) {#setformula-3}

Set the formula and the value of the formula. NOTE: This class is now obsolete. Instead, please use Cell.SetFormula(string,FormulaParseOptions,object). This property will be removed 12 months later since December 2019. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The formula. |
| isR1C1 | boolean | Whether the formula is R1C1 formula. |
| isLocal | boolean | Whether the formula is locale formatted. |
| value | Object | The value of the formula. |

### setFormula(formula, options, value) {#setformula-4}

Set the formula and the value(calculated result) of the formula.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The formula. |
| options | FormulaParseOptions | Options for parsing the formula. |
| value | Object | The value(calculated result) of the formula. |

### setFormulaLocal() {#setformulalocal}

Get the locale formatted formula of the cell.

### setHtmlString() {#sethtmlstring}

Gets and sets the html string which contains data and some formats in this cell.

### setR1C1Formula() {#setr1c1formula}

Gets or sets a R1C1 formula of the Cell.

### setSharedFormula(sharedFormula, rowNumber, columnNumber, isR1C1, isLocal) {#setsharedformula}

Sets a formula to a range of cells. NOTE: This class is now obsolete. Instead, please use Cell.SetSharedFormula(string,int,int,FormulaParseOptions). This property will be removed 12 months later since December 2019. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| sharedFormula | String | Shared formula. |
| rowNumber | Number | Number of rows to populate the formula. |
| columnNumber | Number | Number of columns to populate the formula. |
| isR1C1 | boolean | whether the formula is R1C1 formula |
| isLocal | boolean | whether the formula is locale formatted |

### setSharedFormula(sharedFormula, rowNumber, columnNumber) {#setsharedformula-1}

Sets shared formulas to a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| sharedFormula | String | Shared formula. |
| rowNumber | Number | Number of rows to populate the formula. |
| columnNumber | Number | Number of columns to populate the formula. |

### setSharedFormula(sharedFormula, rowNumber, columnNumber, options) {#setsharedformula-2}

Sets shared formulas to a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| sharedFormula | String | Shared formula. |
| rowNumber | Number | Number of rows to populate the formula. |
| columnNumber | Number | Number of columns to populate the formula. |
| options | FormulaParseOptions | Options for parsing the formula. |

### setSharedFormula(sharedFormula, rowNumber, columnNumber, options, values) {#setsharedformula-3}

Sets shared formulas to a range of cells.

| Parameter | Type | Description |
| --- | --- | --- |
| sharedFormula | String | Shared formula. |
| rowNumber | Number | Number of rows to populate the formula. |
| columnNumber | Number | Number of columns to populate the formula. |
| options | FormulaParseOptions | Options for parsing the formula. |
| values | Array of Array of Object | values for those cells with given shared formula |

### setStyle(style) {#setstyle}

Sets the cell style. If the border settings are changed, the border of adjust cells will be updated too.

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The cell style. |

### setStyle(style, explicitFlag) {#setstyle-1}

Apply the changed property of style to the cell.

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The cell style. |
| explicitFlag | boolean | True, only overwriting formatting which is explicitly set. |

### setStyle(style, flag) {#setstyle-2}

Apply the cell style based on flags.

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The cell style. |
| flag | StyleFlag | The style flag. |

### setTableFormula(rowNumber, columnNumber, rowInputCell, columnInputCell, values) {#settableformula}

Create two-variable data table for given range starting from this cell.

| Parameter | Type | Description |
| --- | --- | --- |
| rowNumber | Number | Number of rows to populate the formula. |
| columnNumber | Number | Number of columns to populate the formula. |
| rowInputCell | String | the row input cell |
| columnInputCell | String | the column input cell |
| values | Array of Array of Object | values for cells in table formula range |

### setTableFormula(rowNumber, columnNumber, inputCell, isRowInput, values) {#settableformula-1}

Create one-variable data table for given range starting from this cell.

| Parameter | Type | Description |
| --- | --- | --- |
| rowNumber | Number | Number of rows to populate the formula. |
| columnNumber | Number | Number of columns to populate the formula. |
| inputCell | String | the input cell |
| isRowInput | boolean | Indicates whether the input cell is a row input cell(true) or a column input cell(false). |
| values | Array of Array of Object | values for cells in table formula range |

### setTableFormula(rowNumber, columnNumber, rowIndexOfRowInputCell, columnIndexOfRowInputCell, rowIndexOfColumnInputCell, columnIndexOfColumnInputCell, values) {#settableformula-2}

Create two-variable data table for given range starting from this cell.

| Parameter | Type | Description |
| --- | --- | --- |
| rowNumber | Number | Number of rows to populate the formula. |
| columnNumber | Number | Number of columns to populate the formula. |
| rowIndexOfRowInputCell | Number | row index of the row input cell |
| columnIndexOfRowInputCell | Number | column index of the row input cell |
| rowIndexOfColumnInputCell | Number | row index of the column input cell |
| columnIndexOfColumnInputCell | Number | column index of the column input cell |
| values | Array of Array of Object | values for cells in table formula range |

### setTableFormula(rowNumber, columnNumber, rowIndexOfInputCell, columnIndexOfInputCell, isRowInput, values) {#settableformula-3}

Create one-variable data table for given range starting from this cell.

| Parameter | Type | Description |
| --- | --- | --- |
| rowNumber | Number | Number of rows to populate the formula. |
| columnNumber | Number | Number of columns to populate the formula. |
| rowIndexOfInputCell | Number | row index of the input cell |
| columnIndexOfInputCell | Number | column index of the input cell |
| isRowInput | boolean | Indicates whether the input cell is a row input cell(true) or a column input cell(false). |
| values | Array of Array of Object | values for cells in table formula range |

### setValue() {#setvalue}

Gets/sets the value contained in this cell. Possible type: null,Boolean,DateTime,Double,IntegerString. For int value, it may be returned as an Integer object or a Double object. And there is no guarantee that the returned value will be kept as the same type of object always.

### toJson() {#tojson}

Convert Cell to JSON struct data.

**Returns:** String — `String`

### toString() {#tostring}

Returns a string represents the current Cell object.

**Returns:** String — `String`
