##Cell.GetLeafs
Cell method. Get all cells which reference to this cell directly and need to be updated when this cell is modified
## GetLeafs() {#getleafs}
Get all cells which reference to this cell directly and need to be updated when this cell is modified.
```csharp
[Obsolete("Use GetDependentsInCalculation(bool) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IEnumerator GetLeafs()
```
### Return Value
Enumerator to enumerate all dependents(Cell)
### Remarks
NOTE: This class is now obsolete. Instead, please use Cell.GetDependentsInCalculation(bool) to get all dependents in calculation chain. This property will be removed 12 months later since May 2022. Aspose apologizes for any inconvenience you may have experienced.
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetLeafs(bool) {#getleafs_1}
Get all cells which will be updated when this cell is modified.
```csharp
[Obsolete("Use GetDependentsInCalculation(bool) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IEnumerator GetLeafs(bool recursive)
```
| Parameter | Type | Description |
| --- | --- | --- |
| recursive | Boolean | Whether returns those leafs that do not reference to this cell directly but reference to other leafs of this cell |
### Return Value
Enumerator to enumerate all dependents(Cell)
### Remarks
NOTE: This class is now obsolete. Instead, please use Cell.GetDependentsInCalculation(bool) to get all dependents in calculation chain. This property will be removed 12 months later since May 2022. Aspose apologizes for any inconvenience you may have experienced.
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
