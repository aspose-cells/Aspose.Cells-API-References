---
title: Cell
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 230
url: /net/aspose.cells/cell/
---
## Cell class

Encapsulates the object that represents a single Workbook cell.

```csharp
public class Cell
```

## Properties

| Name | Description |
| --- | --- |
| [BoolValue](../../aspose.cells/cell/boolvalue) { get; } | Gets the boolean value contained in the cell. |
| [Column](../../aspose.cells/cell/column) { get; } | Gets column number (zero based) of the cell. |
| [Comment](../../aspose.cells/cell/comment) { get; } | Gets the comment of this cell. |
| [ContainsExternalLink](../../aspose.cells/cell/containsexternallink) { get; } | Indicates whether this cell contains an external link. Only applies when the cell is a formula cell. |
| [DateTimeValue](../../aspose.cells/cell/datetimevalue) { get; } | Gets the DateTime value contained in the cell. |
| [DisplayStringValue](../../aspose.cells/cell/displaystringvalue) { get; } | Gets the formatted string value of this cell by cell's display style. |
| [DoubleValue](../../aspose.cells/cell/doublevalue) { get; } | Gets the double value contained in the cell. |
| [FloatValue](../../aspose.cells/cell/floatvalue) { get; } | Gets the float value contained in the cell. |
| [Formula](../../aspose.cells/cell/formula) { get; set; } | Gets or sets a formula of the [`Cell`](../cell). |
| [FormulaLocal](../../aspose.cells/cell/formulalocal) { get; set; } | Get the locale formatted formula of the cell. |
| [HtmlString](../../aspose.cells/cell/htmlstring) { get; set; } | Gets and sets the html string which contains data and some formats in this cell. |
| [IntValue](../../aspose.cells/cell/intvalue) { get; } | Gets the integer value contained in the cell. |
| [IsArrayFormula](../../aspose.cells/cell/isarrayformula) { get; } | Indicates whether the cell formula is an array formula. |
| [IsArrayHeader](../../aspose.cells/cell/isarrayheader) { get; } | Indicates the cell's formula is and array formula and it is the first cell of the array. |
| [IsErrorValue](../../aspose.cells/cell/iserrorvalue) { get; } | Checks if a formula can properly evaluate a result. |
| [IsFormula](../../aspose.cells/cell/isformula) { get; } | Represents if the specified cell contains formula. |
| [IsMerged](../../aspose.cells/cell/ismerged) { get; } | Checks if a cell is part of a merged range or not. |
| [IsNumericValue](../../aspose.cells/cell/isnumericvalue) { get; } | Indicates whether the inner value of this cell is numeric(int, double and datetime) |
| [IsSharedFormula](../../aspose.cells/cell/issharedformula) { get; } | Indicates whether the cell formula is part of shared formula. |
| [IsStyleSet](../../aspose.cells/cell/isstyleset) { get; } | Indicates if the cell's style is set. If return false, it means this cell has a default cell format. |
| [IsTableFormula](../../aspose.cells/cell/istableformula) { get; } | Indicates whether this cell is part of table formula. |
| [Name](../../aspose.cells/cell/name) { get; } | Gets the name of the cell. |
| [NumberCategoryType](../../aspose.cells/cell/numbercategorytype) { get; } | Represents the category type of this cell's number formatting. |
| [R1C1Formula](../../aspose.cells/cell/r1c1formula) { get; set; } | Gets or sets a R1C1 formula of the [`Cell`](../cell). |
| [Row](../../aspose.cells/cell/row) { get; } | Gets row number (zero based) of the cell. |
| [SharedStyleIndex](../../aspose.cells/cell/sharedstyleindex) { get; } | Gets cell's shared style index in the style pool. |
| [StringValue](../../aspose.cells/cell/stringvalue) { get; } | Gets the string value contained in the cell. If the type of this cell is string, then return the string value itself. For other cell types, the formatted string value (formatted with the specified style of this cell) will be returned. The formatted cell value is same with what you can get from excel when copying a cell as text(such as copying cell to text editor or exporting to csv). |
| [Type](../../aspose.cells/cell/type) { get; } | Represents cell value type. |
| [Value](../../aspose.cells/cell/value) { get; set; } | Gets the value contained in this cell. |
| [Worksheet](../../aspose.cells/cell/worksheet) { get; } | Gets the parent worksheet. |

## Methods

| Name | Description |
| --- | --- |
| [Calculate](../../aspose.cells/cell/calculate)(CalculationOptions) | Calculates the formula of the cell. |
| [Characters](../../aspose.cells/cell/characters)(int, int) | Returns a Characters object that represents a range of characters within the cell text. |
| [Copy](../../aspose.cells/cell/copy)(Cell) | Copies data from a source cell. |
| [Equals](../../aspose.cells/cell/equals)(Cell) | Checks whether this object refers to the same cell with another cell object. |
| override [Equals](../../aspose.cells/cell/equals)(object) | Checks whether this object refers to the same cell with another. |
| [GetArrayRange](../../aspose.cells/cell/getarrayrange)() | Gets the array range if the cell's formula is an array formula. |
| [GetCharacters](../../aspose.cells/cell/getcharacters)() | Returns all Characters objects that represents a range of characters within the cell text. |
| [GetCharacters](../../aspose.cells/cell/getcharacters)(bool) | Returns all Characters objects that represents a range of characters within the cell text. |
| [GetConditionalFormattingResult](../../aspose.cells/cell/getconditionalformattingresult)() | Get the result of the conditional formatting. |
| [GetDependents](../../aspose.cells/cell/getdependents)(bool) | Get all cells which reference to the specific cell. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle)() | Gets the display style of the cell. If this cell is also affected by other settings such as conditional formatting, list objects, etc., then the display style may be different from cell.GetStyle(). |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle)(bool) | Gets the display style of the cell. If the cell is conditional formatted, the display style is not same as the cell.GetStyle(). |
| [GetFormatConditions](../../aspose.cells/cell/getformatconditions)() | Gets format conditions which applies to this cell. |
| [GetFormula](../../aspose.cells/cell/getformula)(bool, bool) | Get the formula of this cell. |
| override [GetHashCode](../../aspose.cells/cell/gethashcode)() | Serves as a hash function for a particular type. |
| [GetHeightOfValue](../../aspose.cells/cell/getheightofvalue)() | Gets the height of the value in unit of pixels. |
| [GetHtmlString](../../aspose.cells/cell/gethtmlstring)(bool) | Gets the html string which contains data and some formats in this cell. |
| [GetLeafs](../../aspose.cells/cell/getleafs)() | Get all cells which reference to this cell directly and need to be updated when this cell is modified. |
| [GetLeafs](../../aspose.cells/cell/getleafs)(bool) | Get all cells which will be updated when this cell is modified. |
| [GetMergedRange](../../aspose.cells/cell/getmergedrange)() | Returns a [`Range`](../range) object which represents a merged range. |
| [GetPrecedents](../../aspose.cells/cell/getprecedents)() | Gets all cells or ranges which this cell's formula depends on. |
| [GetStringValue](../../aspose.cells/cell/getstringvalue)(CellValueFormatStrategy) | Gets the string value by specific formatted strategy. |
| [GetStyle](../../aspose.cells/cell/getstyle)() | Gets the cell style. |
| [GetStyle](../../aspose.cells/cell/getstyle)(bool) | If checkBorders is true, check whether other cells' borders will effect the style of this cell. |
| [GetTable](../../aspose.cells/cell/gettable)() | Gets the table which contains this cell. |
| [GetValidation](../../aspose.cells/cell/getvalidation)() | Gets the validation applied to this cell. |
| [GetValidationValue](../../aspose.cells/cell/getvalidationvalue)() | Gets the value of validation which applied to this cell. |
| [GetWidthOfValue](../../aspose.cells/cell/getwidthofvalue)() | Gets the width of the value in unit of pixels. |
| [IsRichText](../../aspose.cells/cell/isrichtext)() | Indicates whether the cell string value is a rich text. |
| [PutValue](../../aspose.cells/cell/putvalue)(bool) | Puts a boolean value into the cell. |
| [PutValue](../../aspose.cells/cell/putvalue)(DateTime) | Puts a DateTime value into the cell. |
| [PutValue](../../aspose.cells/cell/putvalue)(double) | Puts a double value into the cell. |
| [PutValue](../../aspose.cells/cell/putvalue)(int) | Puts an integer value into the cell. |
| [PutValue](../../aspose.cells/cell/putvalue)(object) | Puts an object value into the cell. |
| [PutValue](../../aspose.cells/cell/putvalue)(string) | Puts a string value into the cell. |
| [PutValue](../../aspose.cells/cell/putvalue)(string, bool) | Puts a string value into the cell and converts the value to other data type if appropriate. |
| [PutValue](../../aspose.cells/cell/putvalue)(string, bool, bool) | Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will be reset. |
| [RemoveArrayFormula](../../aspose.cells/cell/removearrayformula)(bool) | Remove array formula. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula)(string, int, int) | Sets an array formula(legacy array formula entered via CTRL+SHIFT+ENTER in ms excel) to a range of cells. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula)(string, int, int, FormulaParseOptions) | Sets an array formula to a range of cells. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula)(string, int, int, FormulaParseOptions, object[][]) | Sets an array formula to a range of cells. |
| [SetCharacters](../../aspose.cells/cell/setcharacters)(FontSetting[]) | Sets rich text format of the cell. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula)(string, FormulaParseOptions, bool) | Sets dynamic array formula and make the formula spill into neighboring cells if possible. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula)(string, FormulaParseOptions, object[][], bool, bool) | Sets dynamic array formula and make the formula spill into neighboring cells if possible. |
| [SetFormula](../../aspose.cells/cell/setformula)(string, object) | Set the formula and the value of the formula. |
| [SetFormula](../../aspose.cells/cell/setformula)(string, FormulaParseOptions, object) | Set the formula and the value of the formula. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula)(string, int, int) | Sets a formula to a range of cells. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula)(string, int, int, FormulaParseOptions) | Sets a formula to a range of cells. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula)(string, int, int, FormulaParseOptions, object[][]) | Sets a formula to a range of cells. |
| [SetStyle](../../aspose.cells/cell/setstyle)(Style) | Sets the cell style. |
| [SetStyle](../../aspose.cells/cell/setstyle)(Style, bool) | Apply the cell style. |
| [SetStyle](../../aspose.cells/cell/setstyle)(Style, StyleFlag) | Apply the cell style. |
| override [ToString](../../aspose.cells/cell/tostring)() | Returns a string represents the current Cell object. |

### Examples

```csharp
[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//Put a string into a cell
Cell cell = cells[0, 0];
cell.PutValue("Hello");

string first = cell.StringValue;
	
//Put an integer into a cell
cell = cells["B1"];
cell.PutValue(12);

int second = cell.IntValue;

//Put a double into a cell
cell = cells[0, 2];
cell.PutValue(-1.234);

double third = cell.DoubleValue;

//Put a formula into a cell
cell = cells["D1"];
cell.Formula = "=B1 + C1";

//Put a combined formula: "sum(average(b1,c1), b1)" to cell at b2
cell = cells["b2"];
cell.Formula = "=sum(average(b1,c1), b1)";

//Set style of a cell
Style style = cell.GetStyle();
//Set background color
style.BackgroundColor = Color.Yellow;
//Set format of a cell
style.Font.Name = "Courier New";
style.VerticalAlignment = TextAlignmentType.Top;
cell.SetStyle(style);



[Visual Basic]

Dim excel as Workbook = new Workbook()
Dim cells as Cells = exce.Worksheets(0).Cells

'Put a string into a cell
Dim cell as Cell = cells(0, 0)
cell.PutValue("Hello")

Dim first as String = cell.StringValue
	
//Put an integer into a cell
cell = cells("B1")
cell.PutValue(12)

Dim second as Integer = cell.IntValue

//Put a double into a cell
cell = cells(0, 2)
cell.PutValue(-1.234)

Dim third as Double = cell.DoubleValue

//Put a formula into a cell
cell = cells("D1")
cell.Formula = "=B1 + C1"

//Put a combined formula: "sum(average(b1,c1), b1)" to cell at b2
cell = cells("b2")
cell.Formula = "=sum(average(b1,c1), b1)"
	
//Set style of a cell
Dim style as Style = cell.GetStyle()

//Set background color
style.BackgroundColor = Color.Yellow
//Set font of a cell
style.Font.Name = "Courier New"
style.VerticalAlignment = TextAlignmentType.Top
cell.SetStyle(style)
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
