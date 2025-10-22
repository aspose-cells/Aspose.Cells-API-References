##GridValidation.LoadValueList
GridValidation method. Loads value list from a DataView object. You can specify the value field and text field of the DataView. Each value and text pair will be combined to one string with a comma between them
## GridValidation.LoadValueList method
Loads value list from a DataView object. You can specify the value field and text field of the DataView. Each value and text pair will be combined to one string, with a comma between them.
```csharp
public void LoadValueList(DataView view, string valueField, string textField, bool valuePrefixText)
```
| Parameter | Type | Description |
| --- | --- | --- |
| view | DataView | The DataView object. |
| valueField | String | The value field name. |
| textField | String | The text field name. |
| valuePrefixText | Boolean | Indicates whether to add a value prefix to each displayed text. |
### See Also
* class [GridValidation](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
