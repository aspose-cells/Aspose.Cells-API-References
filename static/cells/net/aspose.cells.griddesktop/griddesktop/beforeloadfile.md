##GridDesktop.BeforeLoadFile
GridDesktop event. Occurs before workbook loaded from file
## GridDesktop.BeforeLoadFile event
Occurs before workbook loaded from file.
```csharp
public event WorkbookEventHandler BeforeLoadFile;
```
### Examples
```csharp
[C#]
private void gridDesktop1_BeforeLoadFile(object sender, Aspose.Cells.GridDesktop.Event.WorkBookEvents e)
{
MessageBox.Show("before load file!");
}
[Visual Basic]
Private  Sub gridDesktop1_BeforeLoadFile(ByVal sender As Object, ByVal e As Aspose.Cells.GridDesktop.Event.WorkBookEvents) Handles gridDesktop1.CellDataChanged
MessageBox.Show("before load file!")
End Sub
```
### See Also
* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
