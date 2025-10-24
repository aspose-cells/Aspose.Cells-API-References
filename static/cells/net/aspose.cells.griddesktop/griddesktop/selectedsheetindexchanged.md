##GridDesktop.SelectedSheetIndexChanged
GridDesktop event. Occurs when the SelectedSheetIndex property is changed
## GridDesktop.SelectedSheetIndexChanged event
Occurs when the SelectedSheetIndex property is changed.
```csharp
public event EventHandler SelectedSheetIndexChanged;
```
### Examples
```csharp
[C#]
private void gridDesktop1_SelectedSheetIndexChanged(object sender, System.EventArgs e)
{
MessageBox.Show("selected index changed!");
}
[Visual Basic]
Private  Sub gridDesktop1_SelectedSheetIndexChanged(ByVal sender As Object, ByVal e As System.EventArgs) Handles gridDesktop1.SelectedSheetIndexChanged
MessageBox.Show("selected index changed!")
End Sub
```
### See Also
* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)
