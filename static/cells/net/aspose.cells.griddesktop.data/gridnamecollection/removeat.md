##GridNameCollection.RemoveAt
GridNameCollection method. Remove the name at the specific index
## GridNameCollection.RemoveAt method
Remove the name at the specific index.
```csharp
public void RemoveAt(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 |  |
### Remarks
Please make sure that the name is not referred by the other formulas before calling the method. And if the name is referred,please only set Name.RefersTo as null.
### See Also
* class [GridNameCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
