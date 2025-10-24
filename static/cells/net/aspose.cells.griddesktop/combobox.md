##Class ComboBox
Aspose.Cells.GridDesktop.ComboBox class. Represents a cell combobox control
## ComboBox class
Represents a cell combobox control.
```csharp
public class ComboBox : CellControl
```
## Properties
| Name | Description |
| --- | --- |
| [Height](../../aspose.cells.griddesktop/combobox/height/) { get; set; } | Gets or sets the height of the list control. |
| [IsInputable](../../aspose.cells.griddesktop/combobox/isinputable/) { get; set; } | Indicates if the user can input text to the combobox. The inputted text will be saved as the cell's value. The default value is "false". |
| [Items](../../aspose.cells.griddesktop/combobox/items/) { get; } | Gets an object representing the collection of the items contained in this ComboBox. |
| [SelectedIndex](../../aspose.cells.griddesktop/combobox/selectedindex/) { get; set; } | Gets or sets the index specifying the currently selected item. Setting the index will call GridDesktop.RunAllFormulas method automatic if GridDesktop.RecalculateFormulas property is true. |
| [Text](../../aspose.cells.griddesktop/cellcontrol/text/) { get; set; } | Gets or sets the text associated with this control.(Inherited from [`CellControl`](../cellcontrol/).) |
| [Values](../../aspose.cells.griddesktop/combobox/values/) { get; } | Gets an object representing the collection of the values contained in this ComboBox. |
| [Width](../../aspose.cells.griddesktop/combobox/width/) { get; set; } | Gets or sets the width of the list control. |
## Methods
| Name | Description |
| --- | --- |
| [SetSelectedIndex](../../aspose.cells.griddesktop/combobox/setselectedindex/)(int) | Sets the Selected index of the ComboBox. This will not calculate formula. To calculate formula,need to call GridDesktop.RunAllFormulas manually. It will not auto calculate formulas in any case even GridDesktop.RecalculateFormulas is true. |
### See Also
* class [CellControl](../cellcontrol/)
* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)
