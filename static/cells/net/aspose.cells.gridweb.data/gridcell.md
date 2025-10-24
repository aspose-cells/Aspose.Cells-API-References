##Class GridCell
Aspose.Cells.GridWeb.Data.GridCell class. Represents a cell object
## GridCell class
Represents a cell object.
```csharp
public class GridCell
```
## Properties
| Name | Description |
| --- | --- |
| [BoolValue](../../aspose.cells.gridweb.data/gridcell/boolvalue/) { get; } | Gets the boolean value contained in the cell. |
| [Column](../../aspose.cells.gridweb.data/gridcell/column/) { get; } | Gets column number (zero based) of the cell. |
| [DateValue](../../aspose.cells.gridweb.data/gridcell/datevalue/) { get; } | Gets the DateTime value contained in the cell. |
| [DisplayStringValue](../../aspose.cells.gridweb.data/gridcell/displaystringvalue/) { get; } | Gets the formatted string value of this cell. |
| [DoubleValue](../../aspose.cells.gridweb.data/gridcell/doublevalue/) { get; } | Gets the double value contained in the cell. |
| [FloatValue](../../aspose.cells.gridweb.data/gridcell/floatvalue/) { get; } | Gets the float value contained in the cell. |
| [Formula](../../aspose.cells.gridweb.data/gridcell/formula/) { get; set; } | Gets or sets a formula of the `GridCell`. |
| [HtmlString](../../aspose.cells.gridweb.data/gridcell/htmlstring/) { get; set; } | Gets and sets the html string which contains data and some formattings in this cell. |
| [IntValue](../../aspose.cells.gridweb.data/gridcell/intvalue/) { get; } | Gets the integer value contained in the cell. |
| [IsStyleSet](../../aspose.cells.gridweb.data/gridcell/isstyleset/) { get; } | Indicates if the cell's style is set. If return false, it means this cell has a default cell format. |
| [Name](../../aspose.cells.gridweb.data/gridcell/name/) { get; } | Gets the name of the cell. For example: A1, F102. |
| [Row](../../aspose.cells.gridweb.data/gridcell/row/) { get; } | Gets row number (zero based) of the cell. |
| [StringValue](../../aspose.cells.gridweb.data/gridcell/stringvalue/) { get; } | Gets the string value contained in the cell. |
| [Style](../../aspose.cells.gridweb.data/gridcell/style/) { get; set; } | Gets the copy of cell style. set the style for the cell. |
| [Type](../../aspose.cells.gridweb.data/gridcell/type/) { get; } | return the cell value type ,the meaning can see GridCellValueType.java |
| [Value](../../aspose.cells.gridweb.data/gridcell/value/) { get; set; } | Gets the value contained in this cell. |
## Methods
| Name | Description |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.gridweb.data/gridcell/containsexternallink/)() | Indicates wether this cell contains an external link. Only applies when the cell is a formula cell. |
| [Copy](../../aspose.cells.gridweb.data/gridcell/copy/)(GridCell) | Copies data from a source cell. |
| [CopyStyle](../../aspose.cells.gridweb.data/gridcell/copystyle/)(GridTableItemStyle) | copy the style and set the style for the cell |
| [CreateComment](../../aspose.cells.gridweb.data/gridcell/createcomment/)(string, string, bool) | Creates a comment object for a cell. |
| [CreateValidation](../../aspose.cells.gridweb.data/gridcell/createvalidation/)(GridValidationType, bool) | Creates a validation object for a cell. |
| override [Equals](../../aspose.cells.gridweb.data/gridcell/equals/)(object) | Checks whether this object refers to the same cell with another cell object. |
| [GetComment](../../aspose.cells.gridweb.data/gridcell/getcomment/)() | Get comment object on this cell |
| override [GetHashCode](../../aspose.cells.gridweb.data/gridcell/gethashcode/)() | Serves as a hash function for a particular type. |
| [GetWidthOfValue](../../aspose.cells.gridweb.data/gridcell/getwidthofvalue/)() | Gets the width of the value in unit of pixels. |
| [IsErrorValue](../../aspose.cells.gridweb.data/gridcell/iserrorvalue/)() | Checks if a formula can properly evaluate a result. |
| [IsFormula](../../aspose.cells.gridweb.data/gridcell/isformula/)() | Represents if the specified cell contains formula. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue)(bool) | Puts a boolean value into the cell. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_3)(DateTime) | Puts a DateTime value into the cell. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_1)(double) | Puts a double value into the cell. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_2)(int) | Puts a int value into the cell. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_4)(object) | Puts an object value into the cell.same as setValue(Object param_object) |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_5)(string) | Puts a String value into the cell. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_6)(string, bool) | Puts a string value into the cell and converts the value to other data type if appropriate. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_7)(string, bool, bool) | Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will be reset. |
| [PutValueAndSetFormatByValue](../../aspose.cells.gridweb.data/gridcell/putvalueandsetformatbyvalue/)(string) | Sets the cell's value with a string value and set cell format by this value. |
| [RemoveComment](../../aspose.cells.gridweb.data/gridcell/removecomment/)() | Removes the comment object of the cell. |
| [RemoveValidation](../../aspose.cells.gridweb.data/gridcell/removevalidation/)() | Removes the validation object of the cell. |
| [SetBorder](../../aspose.cells.gridweb.data/gridcell/setborder/)(WebBorderStyle) | Sets borders(top,bottom,left and right) for a cell,all the borders have same borderstyle. |
| [SetCustom](../../aspose.cells.gridweb.data/gridcell/setcustom/)(string) | sets the custom format, null or empty string means no custom format. |
| [SetFormula](../../aspose.cells.gridweb.data/gridcell/setformula/)(string, object) | Set the formula and the value of the formula. |
| [SetNumberType](../../aspose.cells.gridweb.data/gridcell/setnumbertype/)(int) | set the display format of numbers and dates |
| [ToString](../../aspose.cells.gridweb.data/gridcell/tostring/#tostring)() | Returns a string represents the current Cell object. |
| [operator ==](../../aspose.cells.gridweb.data/gridcell/op_equality/) |  |
| [operator !=](../../aspose.cells.gridweb.data/gridcell/op_inequality/) |  |
### See Also
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)
