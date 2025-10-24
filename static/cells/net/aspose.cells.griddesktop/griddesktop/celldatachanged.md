##GridDesktop.CellDataChanged
GridDesktop event. Occurs when the grid cell data property is changed
## GridDesktop.CellDataChanged event
Occurs when the grid cell data property is changed.
```csharp
public event CellEventHandler CellDataChanged;
```
### Examples
```csharp
[C#]
private void gridDesktop1_CellDataChanged(object sender, Aspose.Cells.GridDesktop.Event.CellEventArgs e)
{
MessageBox.Show("Cell Data changed!");
}
[Visual Basic]
Private  Sub gridDesktop1_CellDataChanged(ByVal sender As Object, ByVal e As Aspose.Cells.GridDesktop.Event.CellEventArgs) Handles gridDesktop1.CellDataChanged
MessageBox.Show("Cell Data changed!")
End Sub
```
### See Also
* delegate [CellEventHandler](../../celleventhandler/)
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
