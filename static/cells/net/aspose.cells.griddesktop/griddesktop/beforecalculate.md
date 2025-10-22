##GridDesktop.BeforeCalculate
GridDesktop event. Occurs before calculate formula in workbook
## GridDesktop.BeforeCalculate event
Occurs before calculate formula in workbook.
```csharp
public event WorkbookEventHandler BeforeCalculate;
```
### Examples
```csharp
[C#]
private void gridDesktop1_BeforeCalculate(object sender, Aspose.Cells.GridDesktop.Event.WorkBookEvents e)
{
MessageBox.Show("before calculate formula!");
}
[Visual Basic]
Private  Sub gridDesktop1_BeforeCalculate(ByVal sender As Object, ByVal e As Aspose.Cells.GridDesktop.Event.WorkBookEvents) Handles gridDesktop1.CellDataChanged
MessageBox.Show("before calculate formula!")
End Sub
```
### See Also
* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
