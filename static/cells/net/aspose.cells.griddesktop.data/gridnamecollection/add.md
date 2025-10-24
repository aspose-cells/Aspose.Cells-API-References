##GridNameCollection.Add
GridNameCollection method. Defines a new global name
## Add(string, string) {#add_1}
Defines a new global name.
```csharp
public int Add(string text, string refersTo)
```
| Parameter | Type | Description |
| --- | --- | --- |
| text | String | Name text.It can have sheetname . |
| refersTo | String | The formula that the name is defined to refer to.It must have a sheetname .eg.'sheet hello!'A1:B2. |
### Return Value
Name object index.
### See Also
* class [GridNameCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## Add(int, string, string) {#add}
Defines a new name in the specified sheet.
```csharp
public int Add(int sheetIndex, string text, string refersTo)
```
| Parameter | Description |
| --- | --- |
| sheetIndex | The sheet index that the name is applyed in. |
| text | Name text.It can not have sheetname . |
| refersTo | The formula that the name is defined to refer to.It must have sheetname .eg.'sheet hello!'A1:B2. |
| sheetIndex | Name's SheetIndex ,the index is from 1. |
### Return Value
Name object index.
### See Also
* class [GridNameCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
