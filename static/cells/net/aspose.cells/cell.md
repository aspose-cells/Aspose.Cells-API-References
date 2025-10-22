##Class Cell
Aspose.Cells.Cell class. Encapsulates the object that represents a single Workbook cell
## Cell class
Encapsulates the object that represents a single Workbook cell.
```csharp
public class Cell
```
## Properties
| Name | Description |
| --- | --- |
| [BoolValue](../../aspose.cells/cell/boolvalue/) { get; } | Gets the boolean value contained in the cell. |
| [Column](../../aspose.cells/cell/column/) { get; } | Gets column number (zero based) of the cell. |
| [Comment](../../aspose.cells/cell/comment/) { get; } | Gets the comment of this cell. |
| [ContainsExternalLink](../../aspose.cells/cell/containsexternallink/) { get; } | Indicates whether this cell contains an external link. Only applies when the cell is a formula cell. |
| [DateTimeValue](../../aspose.cells/cell/datetimevalue/) { get; } | Gets the DateTime value contained in the cell. |
| [DisplayStringValue](../../aspose.cells/cell/displaystringvalue/) { get; } | Gets the formatted string value of this cell by cell's display style. |
| [DoubleValue](../../aspose.cells/cell/doublevalue/) { get; } | Gets the double value contained in the cell. |
| [EmbeddedImage](../../aspose.cells/cell/embeddedimage/) { get; set; } | Gets and sets the embeddedn image in the cell. |
| [FloatValue](../../aspose.cells/cell/floatvalue/) { get; } | Gets the float value contained in the cell. |
| [Formula](../../aspose.cells/cell/formula/) { get; set; } | Gets or sets a formula of the `Cell`. |
| [FormulaLocal](../../aspose.cells/cell/formulalocal/) { get; set; } | Get the locale formatted formula of the cell. |
| [HasCustomFunction](../../aspose.cells/cell/hascustomfunction/) { get; } | Checks whether there is custom function(unsupported function) in this cell's formula. |
| [HasCustomStyle](../../aspose.cells/cell/hascustomstyle/) { get; } | Indicates whether this cell has custom style settings(different from the default one inherited from corresponding row, column, or workbook). |
| [HtmlString](../../aspose.cells/cell/htmlstring/) { get; set; } | Gets and sets the html string which contains data and some formats in this cell. |
| [IntValue](../../aspose.cells/cell/intvalue/) { get; } | Gets the integer value contained in the cell. |
| [IsArrayFormula](../../aspose.cells/cell/isarrayformula/) { get; } | Indicates whether the cell formula is an array formula. |
| [IsArrayHeader](../../aspose.cells/cell/isarrayheader/) { get; } | Indicates the cell's formula is an array formula and it is the first cell of the array. |
| [IsCheckBoxStyle](../../aspose.cells/cell/ischeckboxstyle/) { get; set; } | Indicates whether setting this cell as a check box. |
| [IsDynamicArrayFormula](../../aspose.cells/cell/isdynamicarrayformula/) { get; } | Indicates whether the cell's formula is dynamic array formula(true) or legacy array formula(false). |
| [IsErrorValue](../../aspose.cells/cell/iserrorvalue/) { get; } | Checks if the value of this cell is an error. |
| [IsFormula](../../aspose.cells/cell/isformula/) { get; } | Represents if the specified cell contains formula. |
| [IsInArray](../../aspose.cells/cell/isinarray/) { get; } | (**Obsolete.**) Indicates whether the cell formula is an array formula. |
| [IsInTable](../../aspose.cells/cell/isintable/) { get; } | (**Obsolete.**) Indicates whether this cell is part of table formula. |
| [IsMerged](../../aspose.cells/cell/ismerged/) { get; } | Checks if a cell is part of a merged range or not. |
| [IsNumericValue](../../aspose.cells/cell/isnumericvalue/) { get; } | Indicates whether the value of this cell is numeric(int, double and datetime) |
| [IsSharedFormula](../../aspose.cells/cell/issharedformula/) { get; } | Indicates whether the cell formula is part of shared formula. |
| [IsStyleSet](../../aspose.cells/cell/isstyleset/) { get; } | Indicates if the cell's style is set. If return false, it means this cell has a default cell format. |
| [IsTableFormula](../../aspose.cells/cell/istableformula/) { get; } | Indicates whether this cell is part of table formula. |
| [Name](../../aspose.cells/cell/name/) { get; } | Gets the name of the cell. |
| [NumberCategoryType](../../aspose.cells/cell/numbercategorytype/) { get; } | Represents the category type of this cell's number formatting. |
| [R1C1Formula](../../aspose.cells/cell/r1c1formula/) { get; set; } | Gets or sets a R1C1 formula of the `Cell`. |
| [Row](../../aspose.cells/cell/row/) { get; } | Gets row number (zero based) of the cell. |
| [SharedStyleIndex](../../aspose.cells/cell/sharedstyleindex/) { get; } | Gets cell's shared style index in the style pool. |
| [StringValue](../../aspose.cells/cell/stringvalue/) { get; } | Gets the string value contained in the cell. If the type of this cell is string, then return the string value itself. For other cell types, the formatted string value (formatted with the specified style of this cell) will be returned. The formatted cell value is same with what you can get from excel when copying a cell as text(such as copying cell to text editor or exporting to csv). |
| [StringValueWithoutFormat](../../aspose.cells/cell/stringvaluewithoutformat/) { get; } | (**Obsolete.**) Gets cell's value as string without any format. |
| [Type](../../aspose.cells/cell/type/) { get; } | Represents cell value type. |
| [Value](../../aspose.cells/cell/value/) { get; set; } | Gets/sets the value contained in this cell. |
| [Worksheet](../../aspose.cells/cell/worksheet/) { get; } | Gets the parent worksheet. |
## Methods
| Name | Description |
| --- | --- |
| [Calculate](../../aspose.cells/cell/calculate/)(CalculationOptions) | Calculates the formula of the cell. |
| [Characters](../../aspose.cells/cell/characters/)(int, int) | Returns a Characters object that represents a range of characters within the cell text. |
| [Copy](../../aspose.cells/cell/copy/)(Cell) | Copies data from a source cell. |
| [Equals](../../aspose.cells/cell/equals/#equals)(Cell) | Checks whether this object refers to the same cell with another cell object. |
| override [Equals](../../aspose.cells/cell/equals/#equals_1)(object) | Checks whether this object refers to the same cell with another. |
| [GetArrayRange](../../aspose.cells/cell/getarrayrange/)() | Gets the array range if the cell's formula is an array formula. |
| [GetCharacters](../../aspose.cells/cell/getcharacters/#getcharacters)() | Returns all Characters objects that represents a range of characters within the cell text. |
| [GetCharacters](../../aspose.cells/cell/getcharacters/#getcharacters_1)(bool) | Returns all Characters objects that represents a range of characters within the cell text. |
| [GetConditionalFormattingResult](../../aspose.cells/cell/getconditionalformattingresult/)() | Get the result of the conditional formatting. |
| [GetDependents](../../aspose.cells/cell/getdependents/)(bool) | Get all cells whose formula references to this cell directly. |
| [GetDependentsInCalculation](../../aspose.cells/cell/getdependentsincalculation/)(bool) | Gets all cells whose calculated result depends on this cell. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle/#getdisplaystyle)() | Gets the display style of this cell. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle/#getdisplaystyle_2)(bool) | Gets the display style of this cell. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle/#getdisplaystyle_1)(BorderType) | Gets the display style of this cell. |
| [GetFormatConditions](../../aspose.cells/cell/getformatconditions/)() | Gets format conditions which applies to this cell. |
| [GetFormula](../../aspose.cells/cell/getformula/)(bool, bool) | Get the formula of this cell. |
| override [GetHashCode](../../aspose.cells/cell/gethashcode/)() | Serves as a hash function for a particular type. |
| [GetHeightOfValue](../../aspose.cells/cell/getheightofvalue/)() | Gets the height of the value in unit of pixels. |
| [GetHtmlString](../../aspose.cells/cell/gethtmlstring/)(bool) | Gets the html string which contains data and some formats in this cell. |
| [GetLeafs](../../aspose.cells/cell/getleafs/#getleafs)() | (**Obsolete.**) Get all cells which reference to this cell directly and need to be updated when this cell is modified. |
| [GetLeafs](../../aspose.cells/cell/getleafs/#getleafs_1)(bool) | (**Obsolete.**) Get all cells which will be updated when this cell is modified. |
| [GetMergedRange](../../aspose.cells/cell/getmergedrange/)() | Returns a [`Range`](../range/) object which represents a merged range. |
| [GetPrecedents](../../aspose.cells/cell/getprecedents/)() | Gets all references appearing in this cell's formula. |
| [GetPrecedentsInCalculation](../../aspose.cells/cell/getprecedentsincalculation/)() | Gets all precedents(reference to cells in current workbook) used by this cell's formula while calculating it. |
| [GetRichValue](../../aspose.cells/cell/getrichvalue/)() | Gets rich value of the cell. |
| [GetStringValue](../../aspose.cells/cell/getstringvalue/)(CellValueFormatStrategy) | Gets the string value by specific formatted strategy. |
| [GetStyle](../../aspose.cells/cell/getstyle/#getstyle)() | Gets the cell style. |
| [GetStyle](../../aspose.cells/cell/getstyle/#getstyle_1)(bool) | If checkBorders is true, check whether other cells' borders will effect the style of this cell. |
| [GetTable](../../aspose.cells/cell/gettable/)() | Gets the table which contains this cell. |
| [GetValidation](../../aspose.cells/cell/getvalidation/)() | Gets the validation applied to this cell. |
| [GetValidationValue](../../aspose.cells/cell/getvalidationvalue/)() | Gets the value of validation which applied to this cell. |
| [GetWidthOfValue](../../aspose.cells/cell/getwidthofvalue/)() | Gets the width of the value in unit of pixels. |
| [InsertText](../../aspose.cells/cell/inserttext/)(int, string) | Insert some characters to the cell. If the cell is rich formatted, this method could keep the original formatting. |
| [IsRichText](../../aspose.cells/cell/isrichtext/)() | Indicates whether the string value of this cell is a rich formatted text. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue)(bool) | Puts a boolean value into the cell. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_3)(DateTime) | Puts a DateTime value into the cell. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_1)(double) | Puts a double value into the cell. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_2)(int) | Puts an integer value into the cell. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_4)(object) | Puts an object value into the cell. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_5)(string) | Puts a string value into the cell. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_6)(string, bool) | Puts a string value into the cell and converts the value to other data type if appropriate. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_7)(string, bool, bool) | Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will be reset. |
| [RemoveArrayFormula](../../aspose.cells/cell/removearrayformula/)(bool) | Remove array formula. |
| [Replace](../../aspose.cells/cell/replace/)(string, string, ReplaceOptions) | Replace text of the cell with options. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula)(string, int, int) | Sets an array formula(legacy array formula entered via CTRL+SHIFT+ENTER in ms excel) to a range of cells. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula_1)(string, int, int, FormulaParseOptions) | Sets an array formula to a range of cells. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula_3)(string, int, int, bool, bool) | (**Obsolete.**) Sets an array formula to a range of cells. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula_2)(string, int, int, FormulaParseOptions, object[][]) | Sets an array formula to a range of cells. |
| [SetCharacters](../../aspose.cells/cell/setcharacters/)(FontSetting[]) | Sets rich text format of the cell. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula/#setdynamicarrayformula)(string, FormulaParseOptions, bool) | Sets dynamic array formula and make the formula spill into neighboring cells if possible. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula/#setdynamicarrayformula_1)(string, FormulaParseOptions, object[][], bool, bool) | Sets dynamic array formula and make the formula spill into neighboring cells if possible. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula/#setdynamicarrayformula_2)(string, FormulaParseOptions, object[][], bool, bool, CalculationOptions) | Sets dynamic array formula and make the formula spill into neighboring cells if possible. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula)(string, FormulaParseOptions) | Set the formula and the value(calculated result) of the formula. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula_3)(string, object) | Set the formula and the value(calculated result) of the formula. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula_1)(string, FormulaParseOptions, object) | Set the formula and the value(calculated result) of the formula. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula_2)(string, bool, bool, object) | (**Obsolete.**) Set the formula and the value of the formula. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula)(string, int, int) | Sets shared formulas to a range of cells. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula_1)(string, int, int, FormulaParseOptions) | Sets shared formulas to a range of cells. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula_3)(string, int, int, bool, bool) | (**Obsolete.**) Sets a formula to a range of cells. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula_2)(string, int, int, FormulaParseOptions, object[][]) | Sets shared formulas to a range of cells. |
| [SetStyle](../../aspose.cells/cell/setstyle/#setstyle)(Style) | Sets the cell style. |
| [SetStyle](../../aspose.cells/cell/setstyle/#setstyle_2)(Style, bool) | Apply the changed property of style to the cell. |
| [SetStyle](../../aspose.cells/cell/setstyle/#setstyle_1)(Style, StyleFlag) | Apply the cell style based on flags. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula_2)(int, int, string, bool, object[][]) | Create one-variable data table for given range starting from this cell. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula_3)(int, int, string, string, object[][]) | Create two-variable data table for given range starting from this cell. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula)(int, int, int, int, bool, object[][]) | Create one-variable data table for given range starting from this cell. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula_1)(int, int, int, int, int, int, object[][]) | Create two-variable data table for given range starting from this cell. |
| [ToJson](../../aspose.cells/cell/tojson/)() | Convert `Cell` to JSON struct data. |
| override [ToString](../../aspose.cells/cell/tostring/)() | Returns a string represents the current Cell object. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellDemo
{
public static void CellExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access the cells collection
Cells cells = worksheet.Cells;
// Put a string into a cell
Cell cell = cells[0, 0];
cell.PutValue("Hello");
// Put an integer into a cell
cell = cells["B1"];
cell.PutValue(12);
// Put a double into a cell
cell = cells[0, 2];
cell.PutValue(-1.234);
// Put a formula into a cell
cell = cells["D1"];
cell.Formula = "=B1 + C1";
// Put a combined formula: "sum(average(b1,c1), b1)" to cell at b2
cell = cells["B2"];
cell.Formula = "=sum(average(b1,c1), b1)";
// Set style of a cell
Style style = cell.GetStyle();
// Set background color
style.BackgroundColor = System.Drawing.Color.Yellow;
// Set font of a cell
style.Font.Name = "Courier New";
style.VerticalAlignment = TextAlignmentType.Top;
cell.SetStyle(style);
// Save the workbook
workbook.Save("CellExample.xlsx");
workbook.Save("CellExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
