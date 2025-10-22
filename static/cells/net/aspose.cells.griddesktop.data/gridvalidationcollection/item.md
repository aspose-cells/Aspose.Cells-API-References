##GridValidationCollection.Item
GridValidationCollection property. Gets the Hyperlink element at the specified index
## GridValidationCollection indexer (1 of 2)
Gets the Hyperlink element at the specified index.
```csharp
public GridValidation this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |
### Return Value
The element at the specified index.
### See Also
* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## GridValidationCollection indexer (2 of 2)
Gets the [`GridValidation`](../../gridvalidation/) element at the specified cell.if no validation ,then return null.
```csharp
public GridValidation this[int row, int column] { get; }
```
| Parameter | Description |
| --- | --- |
| row | The row of the cell. |
| column | The column of the cell. |
### Return Value
The element at the specified index.
### Remarks
If there is not a validation object at specified row column index, this will check the column validation object.
### See Also
* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
