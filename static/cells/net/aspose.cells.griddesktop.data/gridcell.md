##Class GridCell
Aspose.Cells.GridDesktop.Data.GridCell class. Represents a cell object
## GridCell class
Represents a cell object.
```csharp
public class GridCell
```
## Properties
| Name | Description |
| --- | --- |
| [BoolValue](../../aspose.cells.griddesktop.data/gridcell/boolvalue/) { get; } | Gets the boolean value contained in the cell. |
| [Column](../../aspose.cells.griddesktop.data/gridcell/column/) { get; } | Gets column number (zero based) of the cell. |
| [DateValue](../../aspose.cells.griddesktop.data/gridcell/datevalue/) { get; } | Gets the DateTime value contained in the cell. |
| [DisplayStringValue](../../aspose.cells.griddesktop.data/gridcell/displaystringvalue/) { get; } | Gets the formatted string value of this cell. |
| [DoubleValue](../../aspose.cells.griddesktop.data/gridcell/doublevalue/) { get; } | Gets the double value contained in the cell. |
| [FloatValue](../../aspose.cells.griddesktop.data/gridcell/floatvalue/) { get; } | Gets the float value contained in the cell. |
| [Formula](../../aspose.cells.griddesktop.data/gridcell/formula/) { get; set; } | Gets or sets a formula of the Cell. |
| [HasCustomStyle](../../aspose.cells.griddesktop.data/gridcell/hascustomstyle/) { get; } | Indicates whether this cell has custom style settings(different from the default one inherited from corresponding row, column, or workbook). |
| [HtmlString](../../aspose.cells.griddesktop.data/gridcell/htmlstring/) { get; set; } | Gets and sets the html string which contains data and some formattings in this cell. |
| [IntValue](../../aspose.cells.griddesktop.data/gridcell/intvalue/) { get; } | Gets the integer value contained in the cell. |
| [IsStyleSet](../../aspose.cells.griddesktop.data/gridcell/isstyleset/) { get; } | Indicates if the cell's style is set. If return false, it means this cell has a default cell format. |
| [Location](../../aspose.cells.griddesktop.data/gridcell/location/) { get; } |  |
| [Name](../../aspose.cells.griddesktop.data/gridcell/name/) { get; } | Gets the name of the cell. For example: A1, F102. |
| [Protected](../../aspose.cells.griddesktop.data/gridcell/protected/) { get; set; } | Indicates if the cell is protected. If the value is "true", user can not modify the cell through the user interface. This attribute has nothing to do with the Style.CellLocked property and will not be saved to file when grid data exported. The default value is "false". |
| [Row](../../aspose.cells.griddesktop.data/gridcell/row/) { get; } | Gets row number (zero based) of the cell. |
| [StringValue](../../aspose.cells.griddesktop.data/gridcell/stringvalue/) { get; } | Gets the string value contained in the cell. |
| [Style](../../aspose.cells.griddesktop.data/gridcell/style/) { get; set; } | Gets the copy of cell style. set the style for the cell. |
| [Type](../../aspose.cells.griddesktop.data/gridcell/type/) { get; } | return the cell value type ,the meaning can see GridCellValueType.java |
| [Value](../../aspose.cells.griddesktop.data/gridcell/value/) { get; set; } | Gets the value contained in this cell. |
| [Worksheet](../../aspose.cells.griddesktop.data/gridcell/worksheet/) { get; } | Gets worksheet object. |
## Methods
| Name | Description |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.griddesktop.data/gridcell/containsexternallink/)() | Indicates wether this cell contains an external link. Only applies when the cell is a formula cell. |
| [Copy](../../aspose.cells.griddesktop.data/gridcell/copy/)(GridCell) | Copies data from a source cell. |
| [CopyStyle](../../aspose.cells.griddesktop.data/gridcell/copystyle/)(Style) | copy the style and set the style for the cell |
| override [Equals](../../aspose.cells.griddesktop.data/gridcell/equals/)(object) |  |
| [GetCellArea](../../aspose.cells.griddesktop.data/gridcell/getcellarea/)() |  |
| [GetFont](../../aspose.cells.griddesktop.data/gridcell/getfont/)() | Gets cell font. When change the font, you should invoke "SetFont" method, to set font to cell. |
| [GetFontColor](../../aspose.cells.griddesktop.data/gridcell/getfontcolor/)() | Gets cell font color. When change the color,you should invoke "SetFontColor" method, to set font color to cell. |
| override [GetHashCode](../../aspose.cells.griddesktop.data/gridcell/gethashcode/)() |  |
| [GetStyle](../../aspose.cells.griddesktop.data/gridcell/getstyle/)() | Gets cell style. When change the style,you should invoke "SetStyle" method, to set style to cell. |
| [GetValidation](../../aspose.cells.griddesktop.data/gridcell/getvalidation/)() | Gets the validation which applied to this cell.if not set return null. |
| [GetWidthOfValue](../../aspose.cells.griddesktop.data/gridcell/getwidthofvalue/)() | Gets the width of the value in unit of pixels. |
| [GetWorksheet](../../aspose.cells.griddesktop.data/gridcell/getworksheet/)() | Gets the parent worksheet. |
| [IsErrorValue](../../aspose.cells.griddesktop.data/gridcell/iserrorvalue/)() | Checks if a formula can properly evaluate a result. |
| [IsFormula](../../aspose.cells.griddesktop.data/gridcell/isformula/)() | Represents if the specified cell contains formula. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue)(bool) | Puts a boolean value into the cell. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_3)(DateTime) | Puts a DateTime value into the cell. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_1)(double) | Puts a double value into the cell. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_2)(int) | Puts a int value into the cell. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_4)(object) | Puts an object value into the cell.same as setValue(Object param_object) |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_5)(string) | Puts a String value into the cell. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_6)(string, bool) | Puts a string value into the cell and converts the value to other data type if appropriate. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_7)(string, bool, bool) | Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will be reset. |
| [PutValueAndSetFormatByValue](../../aspose.cells.griddesktop.data/gridcell/putvalueandsetformatbyvalue/)(string) | Sets the cell's value with a string value and set cell format by this value. |
| [SetCellValue](../../aspose.cells.griddesktop.data/gridcell/setcellvalue/)(object) | If the value is a formula,this method set cell's value as FormulaType, |
| [SetCustom](../../aspose.cells.griddesktop.data/gridcell/setcustom/)(string) | sets the custom format, null or empty string means no custom format. |
| [SetFont](../../aspose.cells.griddesktop.data/gridcell/setfont/)(Font) | Sets font to cell. To improve performance,implement "SetFont" method, not implement "Font" property. |
| [SetFontColor](../../aspose.cells.griddesktop.data/gridcell/setfontcolor/)(Color) | Sets font color to cell. To improve performance,implement "SetFontColor" method, not implement "FontColor" property. |
| [SetFormula](../../aspose.cells.griddesktop.data/gridcell/setformula/)(string, object) | Set the formula and the value of the formula. |
| [SetNumberType](../../aspose.cells.griddesktop.data/gridcell/setnumbertype/)(int) | set the display format of numbers and dates |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcell/setstyle/)(Style) | Sets style to cell. To improve performance,implement "SetStyle" method, not implement "Style" property. |
| override [ToString](../../aspose.cells.griddesktop.data/gridcell/tostring/)() | Returns a string represents the current Cell object. |
| [operator ==](../../aspose.cells.griddesktop.data/gridcell/op_equality/) |  |
| [operator !=](../../aspose.cells.griddesktop.data/gridcell/op_inequality/) |  |
### See Also
* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)
