##GridReferredArea.GetValue
GridReferredArea method. Gets cell value with given offset from the topleft of this area
## GridReferredArea.GetValue method
Gets cell value with given offset from the top-left of this area.
```csharp
public object GetValue(int rowOffset, int colOffset)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | row offset from the start row of this area |
| colOffset | Int32 | column offset from the start row of this area |
### Return Value
"#REF!" if this area is invalid; "#N/A" if given offset out of this area; Otherwise return the cell value at given position.
### See Also
* class [GridReferredArea](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)
