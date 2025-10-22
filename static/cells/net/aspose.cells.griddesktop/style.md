##Class Style
Aspose.Cells.GridDesktop.Style class. Represents display style of excel documentsuch as fontcoloralignmentborderetc
## Style class
Represents display style of excel document,such as font,color,alignment,border,etc.
```csharp
public class Style
```
## Constructors
| Name | Description |
| --- | --- |
| [Style](style/)(GridDesktop) | create a new Style for the control |
## Properties
| Name | Description |
| --- | --- |
| [BackgroundColor](../../aspose.cells.griddesktop/style/backgroundcolor/) { get; set; } | Gets or sets the cell background color,if style pattern is not set to solid,then it will take affect |
| [CellLocked](../../aspose.cells.griddesktop/style/celllocked/) { get; set; } | Gets or sets a value indicating whether a cell can be modified or not. |
| [Color](../../aspose.cells.griddesktop/style/color/) { get; set; } | Gets or sets the cell shading color. when pattern is none ,it return Color.Empty; when pattern is BackgroundType.Solid,it return ForegroundColor; others it return BackgroundColor |
| [Custom](../../aspose.cells.griddesktop/style/custom/) { get; set; } | Represents the custom number format string of this style object. If the custom number format is not set(For example, the number format is builtin), "" will be returned. |
| [Font](../../aspose.cells.griddesktop/style/font/) { get; set; } | Gets a [`GridFont`](../../aspose.cells.griddesktop.data/gridfont/) object. |
| [ForegroundColor](../../aspose.cells.griddesktop/style/foregroundcolor/) { get; set; } | Gets or sets a style's foreground color. |
| [HAlignment](../../aspose.cells.griddesktop/style/halignment/) { get; set; } | Gets or sets horizontal alignment attribute. |
| [Indent](../../aspose.cells.griddesktop/style/indent/) { get; set; } | Represents the m_IndentLevel level for the cell or range. Can only be an integer from 0 to 15. |
| [NumberType](../../aspose.cells.griddesktop/style/numbertype/) { get; set; } | Gets or sets the display format of numbers and dates. The formatting patterns are different for different regions. |
| [Pattern](../../aspose.cells.griddesktop/style/pattern/) { get; set; } | Gets or sets the cell background pattern type. |
| [Rotation](../../aspose.cells.griddesktop/style/rotation/) { get; set; } | Represents text rotation angle. |
| [Shrink](../../aspose.cells.griddesktop/style/shrink/) { get; set; } | Represents if text automatically shrinks to fit in the available column width. |
| [TextDirection](../../aspose.cells.griddesktop/style/textdirection/) { get; set; } | Gets or sets text direction attribute. |
| [TextWrapped](../../aspose.cells.griddesktop/style/textwrapped/) { get; set; } | Gets or sets a value indicating whether the text within a cell is wrapped. |
| [VAlignment](../../aspose.cells.griddesktop/style/valignment/) { get; set; } | Gets or sets vertical alignment attribute. |
## Methods
| Name | Description |
| --- | --- |
| [Clone](../../aspose.cells.griddesktop/style/clone/)() | Creates and returns a copy of this object. **NOTE:**If you clone a named style, name is not cloned becaule style name must be unique. Therefore, the cloned style will not "equals to" the original style. |
| [SetBorderColor](../../aspose.cells.griddesktop/style/setbordercolor/)(BorderType, Color) | Sets the color of the specified border. |
| [SetBorderLine](../../aspose.cells.griddesktop/style/setborderline/)(BorderType, BorderLineType) | Sets the border line type of the specified border. |
### See Also
* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)
