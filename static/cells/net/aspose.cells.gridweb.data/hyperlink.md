##Class Hyperlink
Aspose.Cells.GridWeb.Data.Hyperlink class.
## Hyperlink class
```csharp
[Obsolete("This class is obsolete; use GridHyperlink instead")]
public class Hyperlink
```
## Properties
| Name | Description |
| --- | --- |
| virtual [ActionType](../../aspose.cells.gridweb.data/hyperlink/actiontype/) { get; set; } | Gets or sets the hyperlink's action type. It may be ActionTpye.UrlLink or ActionType.CellCommand. The UrlLink Type means that the hyperlink is a link to a web page or a mail receipt. For example: "http://www.aspose.com" or "mailto:admin@aspose.com". The CellCommand Type means that the hyperlink will fire a CellCommand event, and you may handle this event. |
| [Area](../../aspose.cells.gridweb.data/hyperlink/area/) { get; } | Gets the range of hyperlink. |
| [CellCommand](../../aspose.cells.gridweb.data/hyperlink/cellcommand/) { get; set; } | Gets or sets the Cell Command name. |
| virtual [DiscardInput](../../aspose.cells.gridweb.data/hyperlink/discardinput/) { get; set; } | Indicates whether to discard user input at client browser when user click this CellCommand hyperlink. Could be used as an "undo" action. |
| virtual [ImageUrl](../../aspose.cells.gridweb.data/hyperlink/imageurl/) { get; set; } | Gets or sets the hyperlink's image url. If sets to null or empty string, the hyperlink will only display it's text. |
| [Target](../../aspose.cells.gridweb.data/hyperlink/target/) { get; set; } |  |
| virtual [Text](../../aspose.cells.gridweb.data/hyperlink/text/) { get; set; } | Gets or sets the displayed text of the hyperlink. |
| virtual [ToolTip](../../aspose.cells.gridweb.data/hyperlink/tooltip/) { get; set; } | Gets or sets the tooltip of the hyperlink. |
| virtual [Url](../../aspose.cells.gridweb.data/hyperlink/url/) { get; set; } | Gets or sets the URL string. |
### See Also
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)
