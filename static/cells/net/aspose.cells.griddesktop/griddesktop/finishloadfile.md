##GridDesktop.FinishLoadFile
GridDesktop event. Occurs when the workbook is loaded
## GridDesktop.FinishLoadFile event
Occurs when the workbook is loaded.
```csharp
public event WorkbookEventHandler FinishLoadFile;
```
### Examples
```csharp
[C#]
private void gridDesktop1_FinishLoadFile(object sender, Aspose.Cells.GridDesktop.WorkBookEvents e)
{
MessageBox.Show("finish load file!");
}
[Visual Basic]
Private  Sub gridDesktop1_FinishLoadFile(ByVal sender As Object, ByVal e As Aspose.Cells.GridDesktop.WorkBookEvents) Handles gridDesktop1.FinishLoadFile
MessageBox.Show("finish load file!")
End Sub
```
### See Also
* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
