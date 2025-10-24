##UnionRange.GetEnumerator
UnionRange method. Gets the enumerator for cells in this Range
## UnionRange.GetEnumerator method
Gets the enumerator for cells in this Range.
```csharp
public IEnumerator GetEnumerator()
```
### Return Value
The cells enumerator
### Remarks
When traversing elements by the returned Enumerator, the cells collection should not be modified(such as operations that will cause new Cell/Row be instantiated or existing Cell/Row be deleted). Otherwise the enumerator may not be able to traverse all cells correctly(some elements may be traversed repeatedly or skipped).
### See Also
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
