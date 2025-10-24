##Enum SetBorderPosition
Aspose.Cells.GridWeb.SetBorderPosition enum. Represents the border position to be set of a cells range
## SetBorderPosition enumeration
Represents the border position to be set of a cells range.
```csharp
public enum SetBorderPosition
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Top | `0` | Top border |
| Bottom | `1` | Bottom border |
| Left | `2` | Left border |
| Right | `3` | Right border |
| HorizontalMiddle | `4` | Bottom border |
| VerticalMiddle | `5` | HorizontalMiddle borders |
| Outline | `6` | VerticalMiddle borders |
| Cross | `7` | Cross borders |
| None | `8` | No borders |
### Examples
```csharp
[C#]
GridWeb GridWeb1=new GridWeb();
GridWeb1.WorkSheets[0].Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, GridWeb1.WorkSheets[0].Cells[0, 0].Style.LeftBorderStyle);
[VB]
GridWeb1.WorkSheets(0).Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, GridWeb1.WorkSheets[0].Cells[0, 0].Style.LeftBorderStyle)
```
### See Also
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)
