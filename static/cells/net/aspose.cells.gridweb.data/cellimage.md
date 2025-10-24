##Class CellImage
Aspose.Cells.GridWeb.Data.CellImage class. Reprensents a hyperlink with image src
## CellImage class
Reprensents a hyperlink with image src.
```csharp
public class CellImage : Hyperlink
```
## Properties
| Name | Description |
| --- | --- |
| virtual [ActionType](../../aspose.cells.gridweb.data/hyperlink/actiontype/) { get; set; } | Gets or sets the hyperlink's action type. It may be ActionTpye.UrlLink or ActionType.CellCommand. The UrlLink Type means that the hyperlink is a link to a web page or a mail receipt. For example: "http://www.aspose.com" or "mailto:admin@aspose.com". The CellCommand Type means that the hyperlink will fire a CellCommand event, and you may handle this event.(Inherited from [`Hyperlink`](../hyperlink/).) |
| [Area](../../aspose.cells.gridweb.data/hyperlink/area/) { get; } | Gets the range of hyperlink.(Inherited from [`Hyperlink`](../hyperlink/).) |
| [CellCommand](../../aspose.cells.gridweb.data/hyperlink/cellcommand/) { get; set; } | Gets or sets the Cell Command name.(Inherited from [`Hyperlink`](../hyperlink/).) |
| virtual [DiscardInput](../../aspose.cells.gridweb.data/hyperlink/discardinput/) { get; set; } | Indicates whether to discard user input at client browser when user click this CellCommand hyperlink. Could be used as an "undo" action.(Inherited from [`Hyperlink`](../hyperlink/).) |
| virtual [ImageUrl](../../aspose.cells.gridweb.data/hyperlink/imageurl/) { get; set; } | Gets or sets the hyperlink's image url. If sets to null or empty string, the hyperlink will only display it's text.(Inherited from [`Hyperlink`](../hyperlink/).) |
| [Target](../../aspose.cells.gridweb.data/hyperlink/target/) { get; set; } | (Inherited from [`Hyperlink`](../hyperlink/).) |
| virtual [Text](../../aspose.cells.gridweb.data/hyperlink/text/) { get; set; } | Gets or sets the displayed text of the hyperlink.(Inherited from [`Hyperlink`](../hyperlink/).) |
| virtual [ToolTip](../../aspose.cells.gridweb.data/hyperlink/tooltip/) { get; set; } | Gets or sets the tooltip of the hyperlink.(Inherited from [`Hyperlink`](../hyperlink/).) |
| virtual [Url](../../aspose.cells.gridweb.data/hyperlink/url/) { get; set; } | Gets or sets the URL string.(Inherited from [`Hyperlink`](../hyperlink/).) |
### See Also
* class [Hyperlink](../hyperlink/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)
