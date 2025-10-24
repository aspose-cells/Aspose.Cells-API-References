##GridDesktop.FinishCalculate
GridDesktop event. Occurs after calculate formula in workbook
## GridDesktop.FinishCalculate event
Occurs after calculate formula in workbook.
```csharp
public event WorkbookEventHandler FinishCalculate;
```
### Examples
```csharp
[C#]
private void gridDesktop1_FinishCalculate(object sender, Aspose.Cells.GridDesktop.Event.WorkBookEvents e)
{
MessageBox.Show("finish calculate formula!");
}
[Visual Basic]
Private  Sub gridDesktop1_FinishCalculate(ByVal sender As Object, ByVal e As Aspose.Cells.GridDesktop.Event.WorkBookEvents) Handles gridDesktop1.CellDataChanged
MessageBox.Show("finish calculate formula!")
End Sub
```
### See Also
* delegate [WorkbookEventHandler](../../workbookeventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
