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
| [calculate(options)](./calculate/) | Calculates the formula of the cell. |
| [characters(startIndex, length)](./characters/) | Returns a Characters object that represents a range of characters within the cell text. This method only works on cell w |
| [containsExternalLink()](./containsexternallink/) | Indicates whether this cell contains an external link. Only applies when the cell is a formula cell. |
| [copy(cell)](./copy/) | Copies data from a source cell. |
| [equals(obj)](./equals/) | Checks whether this object refers to the same cell with another. |
| [equals(cell)](./equals-1/) | Checks whether this object refers to the same cell with another cell object. |
| [getArrayRange()](./getarrayrange/) | Gets the array range if the cell's formula is an array formula. Only applies when the cell's formula is an array formula |
| [getBoolValue()](./getboolvalue/) | Gets the boolean value contained in the cell. |
| [getCharacters()](./getcharacters/) | Returns all Characters objects that represents a range of characters within the cell text. |
| [getCharacters(flag)](./getcharacters-1/) | Returns all Characters objects that represents a range of characters within the cell text. |
| [getColumn()](./getcolumn/) | Gets column number (zero based) of the cell. |
| [getComment()](./getcomment/) | Gets the comment of this cell. If there is no comment applies to the cell, returns null. |
| [getConditionalFormattingResult()](./getconditionalformattingresult/) | Get the result of the conditional formatting. Returns null if no conditional formatting is applied to this cell, |
| [getDateTimeValue()](./getdatetimevalue/) | Gets the DateTime value contained in the cell. |
| [getDependents(isAll)](./getdependents/) | Get all cells whose formula references to this cell directly. If one reference containing this cell appears in one cell' |
| [getDependentsInCalculation(recursive)](./getdependentsincalculation/) | Gets all cells whose calculated result depends on this cell. To use this method, please make sure the workbook has been  |
| [getDisplayStringValue()](./getdisplaystringvalue/) | Gets the formatted string value of this cell by cell's display style. |
| [getDisplayStyle()](./getdisplaystyle/) | Gets the display style of the cell. If this cell is also affected by other settings such as conditional formatting, list |
| [getDisplayStyle(includeMergedBorders)](./getdisplaystyle-1/) | Gets the display style of the cell. If the cell is conditional formatted, the display style is not same as the cell.GetS |
| [getDisplayStyle()](./getdisplaystyle-2/) |  |
| [getDoubleValue()](./getdoublevalue/) | Gets the double value contained in the cell. |
| [getEmbeddedImage()](./getembeddedimage/) | Gets and sets the embeddedn image in the cell. |
| [getFloatValue()](./getfloatvalue/) | Gets the float value contained in the cell. |
| [getFormatConditions()](./getformatconditions/) | Gets format conditions which applies to this cell. |
| [getFormula()](./getformula/) | Gets or sets a formula of the Cell. A formula string always begins with an equal sign (=). And please always use comma(, |
| [getFormula(isR1C1, isLocal)](./getformula-1/) | Get the formula of this cell. |
| [getFormulaLocal()](./getformulalocal/) | Get the locale formatted formula of the cell. |
| [getHeightOfValue()](./getheightofvalue/) | Gets the height of the value in unit of pixels. |
| [getHtmlString()](./gethtmlstring/) | Gets and sets the html string which contains data and some formats in this cell. |
| [getHtmlString(html5)](./gethtmlstring-1/) | Gets the html string which contains data and some formats in this cell. |
| [getIntValue()](./getintvalue/) | Gets the integer value contained in the cell. |
| [getLeafs()](./getleafs/) | Get all cells which reference to this cell directly and need to be updated when this cell is modified. NOTE: This class  |
| [getLeafs(recursive)](./getleafs-1/) | Get all cells which will be updated when this cell is modified. NOTE: This class is now obsolete. Instead, please use Ce |
| [getMergedRange()](./getmergedrange/) | Returns a Range object which represents a merged range. |
| [getName()](./getname/) | Gets the name of the cell. A cell name includes its column letter and row number. For example, the name of a cell in row |
| [getNumberCategoryType()](./getnumbercategorytype/) | Represents the category type of this cell's number formatting. The value of the property is NumberCategoryType integer c |
| [getPrecedents()](./getprecedents/) | Gets all references appearing in this cell's formula. Returns null if this is not a formula cell.All references appearin |
| [getPrecedentsInCalculation()](./getprecedentsincalculation/) | Gets all precedents(reference to cells in current workbook) used by this cell's formula while calculating it. This metho |
| [getR1C1Formula()](./getr1c1formula/) | Gets or sets a R1C1 formula of the Cell. |
| [getRichValue()](./getrichvalue/) |  |
| [getRow()](./getrow/) | Gets row number (zero based) of the cell. Cell row number |
| [getSharedStyleIndex()](./getsharedstyleindex/) | Gets cell's shared style index in the style pool. |
| [getStringValue()](./getstringvalue/) | Gets the string value contained in the cell. If the type of this cell is string, then return the string value itself. Fo |
| [getStringValue(formatStrategy)](./getstringvalue-1/) | Gets the string value by specific formatted strategy. |
| [getStringValueWithoutFormat()](./getstringvaluewithoutformat/) | Gets cell's value as string without any format. NOTE: This method is now obsolete. Instead, User should get the value ob |
| [getStyle()](./getstyle/) | Gets the cell style. To change the style of the cell, please call Cell.SetStyle() method after modifying the returned st |
| [getStyle(checkBorders)](./getstyle-1/) | If checkBorders is true, check whether other cells' borders will effect the style of this cell. |
| [getTable()](./gettable/) | Gets the table which contains this cell. |
| [getType()](./gettype/) | Represents cell value type. The value of the property is CellValueType integer constant. |
| [getValidation()](./getvalidation/) | Gets the validation applied to this cell. |
| [getValidationValue()](./getvalidationvalue/) | Gets the value of validation which applied to this cell. |
| [getValue()](./getvalue/) | Gets/sets the value contained in this cell. Possible type: null,Boolean,DateTime,Double,IntegerString. For int value, it |
| [getWidthOfValue()](./getwidthofvalue/) | Gets the width of the value in unit of pixels. |
| [getWorksheet()](./getworksheet/) | Gets the parent worksheet. |
| [hasCustomFunction()](./hascustomfunction/) |  |
| [hasCustomStyle()](./hascustomstyle/) | Indicates whether this cell has custom style settings(different from the default one inherited from corresponding row, c |
| [hashCode()](./hashcode/) | Serves as a hash function for a particular type. |
| [insertText(index, text)](./inserttext/) | Insert some characters to the cell. If the cell is rich formatted, this method could keep the original formatting. |
| [isArrayFormula()](./isarrayformula/) | Indicates whether the cell formula is an array formula. |
| [isArrayHeader()](./isarrayheader/) | Indicates the cell's formula is an array formula and it is the first cell of the array. |
| [isCheckBoxStyle()](./ischeckboxstyle/) |  |
| [isDynamicArrayFormula()](./isdynamicarrayformula/) | Indicates whether the cell's formula is dynamic array formula(true) or legacy array formula(false). |
| [isErrorValue()](./iserrorvalue/) | Checks if the value of this cell is an error. Also applies to formula cell to check whether the calculated result is an  |
| [isFormula()](./isformula/) | Represents if the specified cell contains formula. |
| [isInArray()](./isinarray/) | Indicates whether the cell formula is an array formula. NOTE: This class is now obsolete. Instead, please use Cell.IsArr |
| [isInTable()](./isintable/) | Indicates whether this cell is part of table formula. NOTE: This class is now obsolete. Instead, please use Cell.IsTable |
| [isMerged()](./ismerged/) | Checks if a cell is part of a merged range or not. |
| [isNumericValue()](./isnumericvalue/) | Indicates whether the value of this cell is numeric(int, double and datetime) Also applies to formula cell to check the  |
| [isRichText()](./isrichtext/) | Indicates whether the string value of this cell is a rich formatted text. |
| [isSharedFormula()](./issharedformula/) | Indicates whether the cell formula is part of shared formula. |
| [isStyleSet()](./isstyleset/) | Indicates if the cell's style is set. If return false, it means this cell has a default cell format. |
| [isTableFormula()](./istableformula/) | Indicates whether this cell is part of table formula. |
| [putValue(boolValue)](./putvalue/) | Puts a boolean value into the cell. |
| [putValue(intValue)](./putvalue-1/) | Puts an integer value into the cell. |
| [putValue(doubleValue)](./putvalue-2/) | Puts a double value into the cell. |
| [putValue(stringValue, isConverted, setStyle)](./putvalue-3/) | Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will  |
| [putValue(stringValue, isConverted)](./putvalue-4/) | Puts a string value into the cell and converts the value to other data type if appropriate. |
| [putValue(stringValue)](./putvalue-5/) | Puts a string value into the cell. |
| [putValue(dateTime)](./putvalue-6/) | Puts a DateTime value into the cell. Setting a DateTime value for a cell dose not means the cell will be formatted as da |
| [putValue(objectValue)](./putvalue-7/) | Puts an object value into the cell. |
| [removeArrayFormula(leaveNormalFormula)](./removearrayformula/) | Remove array formula. |
| [replace(placeHolder, newValue, options)](./replace/) | Replace text of the cell with options. |
| [setArrayFormula(arrayFormula, rowNumber, columnNumber, isR1C1, isLocal)](./setarrayformula/) | Sets an array formula to a range of cells. NOTE: This class is now obsolete. Instead, please use Cell.SetArrayFormula(st |
| [setArrayFormula(arrayFormula, rowNumber, columnNumber)](./setarrayformula-1/) | Sets an array formula(legacy array formula entered via CTRL+SHIFT+ENTER in ms excel) to a range of cells. |
| [setArrayFormula(arrayFormula, rowNumber, columnNumber, options)](./setarrayformula-2/) | Sets an array formula to a range of cells. |
| [setArrayFormula(arrayFormula, rowNumber, columnNumber, options, values)](./setarrayformula-3/) | Sets an array formula to a range of cells. |
| [setCharacters(characters)](./setcharacters/) | Sets rich text format of the cell. |
| [setCheckBoxStyle()](./setcheckboxstyle/) |  |
| [setDynamicArrayFormula(arrayFormula, options, calculateValue)](./setdynamicarrayformula/) | Sets dynamic array formula and make the formula spill into neighboring cells if possible. |
| [setDynamicArrayFormula(arrayFormula, options, values, calculateRange, calculateValue)](./setdynamicarrayformula-1/) | Sets dynamic array formula and make the formula spill into neighboring cells if possible. |
| [setDynamicArrayFormula(arrayFormula, options, values, calculateRange, calculateValue, copts)](./setdynamicarrayformula-2/) | Sets dynamic array formula and make the formula spill into neighboring cells if possible. |
| [setEmbeddedImage()](./setembeddedimage/) | Gets and sets the embeddedn image in the cell. |
| [setFormula()](./setformula/) | Gets or sets a formula of the Cell. A formula string always begins with an equal sign (=). And please always use comma(, |
| [setFormula(formula, value)](./setformula-1/) | Set the formula and the value(calculated result) of the formula. |
| [setFormula()](./setformula-2/) |  |
| [setFormula(formula, isR1C1, isLocal, value)](./setformula-3/) | Set the formula and the value of the formula. NOTE: This class is now obsolete. Instead, please use Cell.SetFormula(stri |
| [setFormula(formula, options, value)](./setformula-4/) | Set the formula and the value(calculated result) of the formula. |
| [setFormulaLocal()](./setformulalocal/) | Get the locale formatted formula of the cell. |
| [setHtmlString()](./sethtmlstring/) | Gets and sets the html string which contains data and some formats in this cell. |
| [setR1C1Formula()](./setr1c1formula/) | Gets or sets a R1C1 formula of the Cell. |
| [setSharedFormula(sharedFormula, rowNumber, columnNumber, isR1C1, isLocal)](./setsharedformula/) | Sets a formula to a range of cells. NOTE: This class is now obsolete. Instead, please use Cell.SetSharedFormula(string,i |
| [setSharedFormula(sharedFormula, rowNumber, columnNumber)](./setsharedformula-1/) | Sets shared formulas to a range of cells. |
| [setSharedFormula(sharedFormula, rowNumber, columnNumber, options)](./setsharedformula-2/) | Sets shared formulas to a range of cells. |
| [setSharedFormula(sharedFormula, rowNumber, columnNumber, options, values)](./setsharedformula-3/) | Sets shared formulas to a range of cells. |
| [setStyle(style)](./setstyle/) | Sets the cell style. If the border settings are changed, the border of adjust cells will be updated too. |
| [setStyle(style, explicitFlag)](./setstyle-1/) | Apply the changed property of style to the cell. |
| [setStyle(style, flag)](./setstyle-2/) | Apply the cell style based on flags. |
| [setTableFormula(rowNumber, columnNumber, rowInputCell, columnInputCell, values)](./settableformula/) | Create two-variable data table for given range starting from this cell. |
| [setTableFormula(rowNumber, columnNumber, inputCell, isRowInput, values)](./settableformula-1/) | Create one-variable data table for given range starting from this cell. |
| [setTableFormula(rowNumber, columnNumber, rowIndexOfRowInputCell, columnIndexOfRowInputCell, rowIndexOfColumnInputCell, columnIndexOfColumnInputCell, values)](./settableformula-2/) | Create two-variable data table for given range starting from this cell. |
| [setTableFormula(rowNumber, columnNumber, rowIndexOfInputCell, columnIndexOfInputCell, isRowInput, values)](./settableformula-3/) | Create one-variable data table for given range starting from this cell. |
| [setValue()](./setvalue/) | Gets/sets the value contained in this cell. Possible type: null,Boolean,DateTime,Double,IntegerString. For int value, it |
| [toJson()](./tojson/) | Convert Cell to JSON struct data. |
| [toString()](./tostring/) | Returns a string represents the current Cell object. |
