---
title: Aspose::Cells::Cell class
linktitle: Cell
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Cell class. Encapsulates the object that represents a single Workbook cell in C++.'
type: docs
weight: 1200
url: /cpp/aspose.cells/cell/
---
## Cell class


Encapsulates the object that represents a single [Workbook](../workbook/) cell.

```cpp
class Cell
```

## Methods

| Method | Description |
| --- | --- |
| [Calculate(const CalculationOptions\& options)](./calculate/) | Calculates the formula of the cell. |
| [Cell(Cell_Impl* impl)](./cell/) | Constructs from an implementation object. |
| [Cell(const Cell\& src)](./cell/) | Copy constructor. |
| [Characters(int32_t startIndex, int32_t length)](./characters/) | Returns a Characters object that represents a range of characters within the cell text. |
| [Copy(const Cell\& cell)](./copy/) | Copies data from a source cell. |
| [Dispose()](./dispose/) |  |
| [Equals(const Cell\& cell)](./equals/) | Checks whether this object refers to the same cell with another cell object. |
| [GetArrayRange()](./getarrayrange/) | Gets the array range if the cell's formula is an array formula. |
| [GetBoolValue()](./getboolvalue/) | Gets the boolean value contained in the cell. |
| [GetCharacters()](./getcharacters/) | Returns all Characters objects that represents a range of characters within the cell text. |
| [GetCharacters(bool flag)](./getcharacters/) | Returns all Characters objects that represents a range of characters within the cell text. |
| [GetColumn()](./getcolumn/) | Gets column number (zero based) of the cell. |
| [GetComment()](./getcomment/) | Gets the comment of this cell. |
| [GetConditionalFormattingResult()](./getconditionalformattingresult/) | Get the result of the conditional formatting. |
| [GetContainsExternalLink()](./getcontainsexternallink/) | Indicates whether this cell contains an external link. Only applies when the cell is a formula cell. |
| [GetDateTimeValue()](./getdatetimevalue/) | Gets the DateTime value contained in the cell. |
| [GetDependents(bool isAll)](./getdependents/) | Get all cells whose formula references to this cell directly. |
| [GetDependentsInCalculation(bool recursive)](./getdependentsincalculation/) | Gets all cells whose calculated result depends on this cell. |
| [GetDisplayStringValue()](./getdisplaystringvalue/) | Gets the formatted string value of this cell by cell's display style. |
| [GetDisplayStyle()](./getdisplaystyle/) | Gets the display style of the cell. If this cell is also affected by other settings such as conditional formatting, list objects, etc., then the display style may be different from cell.GetStyle(). |
| [GetDisplayStyle(bool includeMergedBorders)](./getdisplaystyle/) | Gets the display style of the cell. If the cell is conditional formatted, the display style is not same as the cell.GetStyle(). |
| [GetDoubleValue()](./getdoublevalue/) | Gets the double value contained in the cell. |
| [GetFloatValue()](./getfloatvalue/) | Gets the float value contained in the cell. |
| [GetFormatConditions()](./getformatconditions/) | Gets format conditions which applies to this cell. |
| [GetFormula()](./getformula/) | Gets or sets a formula of the [Cell](./). |
| [GetFormula(bool isR1C1, bool isLocal)](./getformula/) | Get the formula of this cell. |
| [GetFormulaLocal()](./getformulalocal/) | Get the locale formatted formula of the cell. |
| [GetHasCustomStyle()](./gethascustomstyle/) | Indicates whether this cell has custom style settings(different from the default one inherited from corresponding row, column, or workbook). |
| [GetHashCode()](./gethashcode/) | Serves as a hash function for a particular type. |
| [GetHeightOfValue()](./getheightofvalue/) | Gets the height of the value in unit of pixels. |
| [GetHtmlString()](./gethtmlstring/) | Gets and sets the html string which contains data and some formats in this cell. |
| [GetHtmlString(bool html5)](./gethtmlstring/) | Gets the html string which contains data and some formats in this cell. |
| [GetIntValue()](./getintvalue/) | Gets the integer value contained in the cell. |
| [GetMergedRange()](./getmergedrange/) | Returns a [Range](../range/) object which represents a merged range. |
| [GetName()](./getname/) | Gets the name of the cell. |
| [GetNumberCategoryType()](./getnumbercategorytype/) | Represents the category type of this cell's number formatting. |
| [GetPrecedents()](./getprecedents/) | Gets all references appearing in this cell's formula. |
| [GetPrecedentsInCalculation()](./getprecedentsincalculation/) | Gets all precedents(reference to cells in current workbook) used by this cell's formula while calculating it. |
| [GetR1C1Formula()](./getr1c1formula/) | Gets or sets a R1C1 formula of the [Cell](./). |
| [GetRow()](./getrow/) | Gets row number (zero based) of the cell. |
| [GetSharedStyleIndex()](./getsharedstyleindex/) | Gets cell's shared style index in the style pool. |
| [GetStringValue(CellValueFormatStrategy formatStrategy)](./getstringvalue/) | Gets the string value by specific formatted strategy. |
| [GetStringValue()](./getstringvalue/) | Gets the string value contained in the cell. If the type of this cell is string, then return the string value itself. For other cell types, the formatted string value (formatted with the specified style of this cell) will be returned. The formatted cell value is same with what you can get from excel when copying a cell as text(such as copying cell to text editor or exporting to csv). |
| [GetStyle()](./getstyle/) | Gets the cell style. |
| [GetStyle(bool checkBorders)](./getstyle/) | If checkBorders is true, check whether other cells' borders will effect the style of this cell. |
| [GetTable()](./gettable/) | Gets the table which contains this cell. |
| [GetType()](./gettype/) | Represents cell value type. |
| [GetValidation()](./getvalidation/) | Gets the validation applied to this cell. |
| [GetValidationValue()](./getvalidationvalue/) | Gets the value of validation which applied to this cell. |
| [GetWidthOfValue()](./getwidthofvalue/) | Gets the width of the value in unit of pixels. |
| [GetWorksheet()](./getworksheet/) | Gets the parent worksheet. |
| [InsertText(int32_t index, const U16String\& text)](./inserttext/) | Insert some characters to the cell. If the cell is rich formatted, this method could keep the original formatting. |
| [InsertText(int32_t index, const char16_t* text)](./inserttext/) | Insert some characters to the cell. If the cell is rich formatted, this method could keep the original formatting. |
| [IsArrayFormula()](./isarrayformula/) | Indicates whether the cell formula is an array formula. |
| [IsArrayHeader()](./isarrayheader/) | Indicates the cell's formula is and array formula and it is the first cell of the array. |
| [IsDynamicArrayFormula()](./isdynamicarrayformula/) | Indicates whether the cell's formula is dynamic array formula(true) or legacy array formula(false). |
| [IsErrorValue()](./iserrorvalue/) | Checks if the value of this cell is an error. |
| [IsFormula()](./isformula/) | Represents if the specified cell contains formula. |
| [IsMerged()](./ismerged/) | Checks if a cell is part of a merged range or not. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsNumericValue()](./isnumericvalue/) | Indicates whether the inner value of this cell is numeric(int, double and datetime) |
| [IsRichText()](./isrichtext/) | Indicates whether the cell string value is a rich text. |
| [IsSharedFormula()](./issharedformula/) | Indicates whether the cell formula is part of shared formula. |
| [IsStyleSet()](./isstyleset/) | Indicates if the cell's style is set. If return false, it means this cell has a default cell format. |
| [IsTableFormula()](./istableformula/) | Indicates whether this cell is part of table formula. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Cell\& src)](./operator_asm/) | operator= |
| [PutValue(bool boolValue)](./putvalue/) | Puts a boolean value into the cell. |
| [PutValue(int32_t intValue)](./putvalue/) | Puts an integer value into the cell. |
| [PutValue(double doubleValue)](./putvalue/) | Puts a double value into the cell. |
| [PutValue(const U16String\& stringValue, bool isConverted, bool setStyle)](./putvalue/) | Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will be reset. |
| [PutValue(const char16_t* stringValue, bool isConverted, bool setStyle)](./putvalue/) | Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will be reset. |
| [PutValue(const U16String\& stringValue, bool isConverted)](./putvalue/) | Puts a string value into the cell and converts the value to other data type if appropriate. |
| [PutValue(const char16_t* stringValue, bool isConverted)](./putvalue/) | Puts a string value into the cell and converts the value to other data type if appropriate. |
| [PutValue(const U16String\& stringValue)](./putvalue/) | Puts a string value into the cell. |
| [PutValue(const char16_t* stringValue)](./putvalue/) | Puts a string value into the cell. |
| [PutValue(const Date\& dateTime)](./putvalue/) | Puts a DateTime value into the cell. |
| [RemoveArrayFormula(bool leaveNormalFormula)](./removearrayformula/) | Remove array formula. |
| [Replace(const U16String\& placeHolder, const U16String\& newValue, const ReplaceOptions\& options)](./replace/) | Replace text of the cell with options. |
| [Replace(const char16_t* placeHolder, const char16_t* newValue, const ReplaceOptions\& options)](./replace/) | Replace text of the cell with options. |
| [SetArrayFormula(const U16String\& arrayFormula, int32_t rowNumber, int32_t columnNumber)](./setarrayformula/) | Sets an array formula(legacy array formula entered via CTRL+SHIFT+ENTER in ms excel) to a range of cells. |
| [SetArrayFormula(const char16_t* arrayFormula, int32_t rowNumber, int32_t columnNumber)](./setarrayformula/) | Sets an array formula(legacy array formula entered via CTRL+SHIFT+ENTER in ms excel) to a range of cells. |
| [SetArrayFormula(const U16String\& arrayFormula, int32_t rowNumber, int32_t columnNumber, const FormulaParseOptions\& options)](./setarrayformula/) | Sets an array formula to a range of cells. |
| [SetArrayFormula(const char16_t* arrayFormula, int32_t rowNumber, int32_t columnNumber, const FormulaParseOptions\& options)](./setarrayformula/) | Sets an array formula to a range of cells. |
| [SetCharacters(const Vector \<FontSetting\>\& characters)](./setcharacters/) | Sets rich text format of the cell. |
| [SetDynamicArrayFormula(const U16String\& arrayFormula, const FormulaParseOptions\& options, bool calculateValue)](./setdynamicarrayformula/) | Sets dynamic array formula and make the formula spill into neighboring cells if possible. |
| [SetDynamicArrayFormula(const char16_t* arrayFormula, const FormulaParseOptions\& options, bool calculateValue)](./setdynamicarrayformula/) | Sets dynamic array formula and make the formula spill into neighboring cells if possible. |
| [SetFormula(const U16String\& value)](./setformula/) | Gets or sets a formula of the [Cell](./). |
| [SetFormula(const char16_t* value)](./setformula/) | Gets or sets a formula of the [Cell](./). |
| [SetFormulaLocal(const U16String\& value)](./setformulalocal/) | Get the locale formatted formula of the cell. |
| [SetFormulaLocal(const char16_t* value)](./setformulalocal/) | Get the locale formatted formula of the cell. |
| [SetHtmlString(const U16String\& value)](./sethtmlstring/) | Gets and sets the html string which contains data and some formats in this cell. |
| [SetHtmlString(const char16_t* value)](./sethtmlstring/) | Gets and sets the html string which contains data and some formats in this cell. |
| [SetR1C1Formula(const U16String\& value)](./setr1c1formula/) | Gets or sets a R1C1 formula of the [Cell](./). |
| [SetR1C1Formula(const char16_t* value)](./setr1c1formula/) | Gets or sets a R1C1 formula of the [Cell](./). |
| [SetSharedFormula(const U16String\& sharedFormula, int32_t rowNumber, int32_t columnNumber)](./setsharedformula/) | Sets shared formulas to a range of cells. |
| [SetSharedFormula(const char16_t* sharedFormula, int32_t rowNumber, int32_t columnNumber)](./setsharedformula/) | Sets shared formulas to a range of cells. |
| [SetSharedFormula(const U16String\& sharedFormula, int32_t rowNumber, int32_t columnNumber, const FormulaParseOptions\& options)](./setsharedformula/) | Sets shared formulas to a range of cells. |
| [SetSharedFormula(const char16_t* sharedFormula, int32_t rowNumber, int32_t columnNumber, const FormulaParseOptions\& options)](./setsharedformula/) | Sets shared formulas to a range of cells. |
| [SetStyle(const Style\& style)](./setstyle/) | Sets the cell style. |
| [SetStyle(const Style\& style, bool explicitFlag)](./setstyle/) | Apply the cell style. |
| [SetStyle(const Style\& style, const StyleFlag\& flag)](./setstyle/) | Apply the cell style. |
| [ToJson()](./tojson/) | Convert [Cell](./) to JSON struct data. |
| [ToString()](./tostring/) | Returns a string represents the current [Cell](./) object. |
| [~Cell()](./~cell/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
Workbook excel;
Cells cells = excel.GetWorksheets().Get(0).GetCells();

//Put a string into a cell
Cell cell = cells.Get(0, 0);
cell.PutValue(u"Hello");

U16String first = cell.GetStringValue();

//Put an integer into a cell
cell = cells.Get(u"B1");
cell.PutValue(12);

int second = cell.GetIntValue();

//Put a double into a cell
cell = cells.Get(0, 2);
cell.PutValue(-1.234);

double third = cell.GetDoubleValue();

//Put a formula into a cell
cell = cells.Get(u"D1");
cell.SetFormula(u"=B1 + C1");

//Put a combined formula: "sum(average(b1,c1), b1)" to cell at b2
cell = cells.Get(u"b2");
cell.SetFormula(u"=sum(average(b1,c1), b1)");

//Set style of a cell
Style style = cell.GetStyle();
//Set background color
style.SetBackgroundColor(Color{ 0xff, 0xff, 0xff, 0 });
//Set format of a cell
style.GetFont().SetName(u"Courier New");
style.SetVerticalAlignment(TextAlignmentType::Top);
cell.SetStyle(style);
Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
