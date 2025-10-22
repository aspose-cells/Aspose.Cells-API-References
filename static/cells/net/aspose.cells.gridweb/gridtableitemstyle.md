##Class GridTableItemStyle
Aspose.Cells.GridWeb.GridTableItemStyle class. Inherited from System.Web.UI.WebControls.TableItemStyle. Encapsulates the styles of a WebCell
## GridTableItemStyle class
Inherited from System.Web.UI.WebControls.TableItemStyle. Encapsulates the styles of a WebCell.
```csharp
public class GridTableItemStyle : TableItemStyle, ISerializable
```
## Constructors
| Name | Description |
| --- | --- |
| [GridTableItemStyle](gridtableitemstyle/)() | Default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [BackImageAttributes](../../aspose.cells.gridweb/gridtableitemstyle/backimageattributes/) { get; set; } | Background image attributes. |
| [BackImageUrl](../../aspose.cells.gridweb/gridtableitemstyle/backimageurl/) { get; set; } | Background image url. |
| [BottomBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/bottomborderstyle/) { get; set; } | Specifies the style of the cell's bottom border. |
| [Custom](../../aspose.cells.gridweb/gridtableitemstyle/custom/) { get; set; } | Gets or sets the custom format, null or empty string means no custom format. |
| [IndentLevel](../../aspose.cells.gridweb/gridtableitemstyle/indentlevel/) { get; set; } | Gets or sets indent level. |
| [IsLocked](../../aspose.cells.gridweb/gridtableitemstyle/islocked/) { get; set; } | Gets or sets a value indicating whether a cell can be modified or not when its worksheet is protected. When its worksheet is protected and IsLocked is true, the cell can not be edit. When its worksheet is protected and IsLocked is false, the cell can be edit. |
| [LeftBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/leftborderstyle/) { get; set; } | Specifies the style of the cell's left border. |
| [NumberType](../../aspose.cells.gridweb/gridtableitemstyle/numbertype/) { get; set; } | Gets or sets the display format of numbers and dates. The formatting patterns are different for different regions. |
| [QuotePrefix](../../aspose.cells.gridweb/gridtableitemstyle/quoteprefix/) { get; set; } | Indicates whether the cell's value starts with single quote mark. |
| [RightBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/rightborderstyle/) { get; set; } | Specifies the style of the cell's right border. |
| [RotationAngle](../../aspose.cells.gridweb/gridtableitemstyle/rotationangle/) { get; set; } | Gets or sets Rotation attribute. |
| [TopBorderStyle](../../aspose.cells.gridweb/gridtableitemstyle/topborderstyle/) { get; set; } | Specifies the style of the cell's top border. |
## Methods
| Name | Description |
| --- | --- |
| override [AddAttributesToRender](../../aspose.cells.gridweb/gridtableitemstyle/addattributestorender/#addattributestorender_1)(HtmlTextWriter, WebControl) | Internal use only. Implementation method Do not call this method directly. |
| override [CopyFrom](../../aspose.cells.gridweb/gridtableitemstyle/copyfrom/)(Style) | Copies from another style object. |
| override [GetHashCode](../../aspose.cells.gridweb/gridtableitemstyle/gethashcode/)() | Serves as a hash function for a particular type, suitable for use in hashing algorithms and data structures like a hash table. |
| override [MergeWith](../../aspose.cells.gridweb/gridtableitemstyle/mergewith/)(Style) | Merges with another style object. |
### Examples
```csharp
[C#]
GridWeb GridWeb1 = new GridWeb();
GridWorksheetCollection sheets = GridWeb1.WorkSheets;
GridWorksheet sheet = sheets.Add("demo1");
sheet.Cells[0,0].PutValue("Demo Text");
GridTableItemStyle style = sheet.Cells[0, 0].Style;
style.Font.Size = FontUnit.Point(72);
style.Wrap = false;
style.BackColor = Color.Gray;
style.BorderStyle = BorderStyle.Solid;
style.BorderWidth = Unit.Pixel(1);
style.BorderColor = Color.Silver;
style.RightBorderStyle.BorderColor = Color.Black;
style.RightBorderStyle.BorderStyle = BorderStyle.Solid;
style.RightBorderStyle.BorderWidth = Unit.Pixel(1);
style.BottomBorderStyle.BorderColor = Color.Black;
style.BottomBorderStyle.BorderStyle = BorderStyle.Solid;
style.BottomBorderStyle.BorderWidth = Unit.Pixel(1);
sheet.Cells[0, 0].Style=style;
[Visual Basic]
Dim sheets As GridWorksheetCollection =  GridWeb1.WorkSheets
Dim sheet As GridWorksheet =  sheets(sheets.Add(__0__))
Dim cell As GridCell =  sheet.Cells(0,0)
cell.StringValue = "Demo Text"
Dim style As GridTableItemStyle = cell.GetStyle()
style.Font.Size = FontUnit.Point(72)
style.Wrap = False
style.BackColor = Color.Gray
style.BorderStyle = BorderStyle.Solid
style.BorderWidth = Unit.Pixel(1)
style.BorderColor = Color.Silver
style.RightBorderStyle.BorderColor = Color.Black
style.RightBorderStyle.BorderStyle = BorderStyle.Solid
style.RightBorderStyle.BorderWidth = Unit.Pixel(1)
style.BottomBorderStyle.BorderColor = Color.Black
style.BottomBorderStyle.BorderStyle = BorderStyle.Solid
style.BottomBorderStyle.BorderWidth = Unit.Pixel(1)
cell.SetStyle(style)
```
### See Also
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)
