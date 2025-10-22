##Aspose::Cells::UnionRange::GetEnumerator method
'Aspose::Cells::UnionRange::GetEnumerator method. Gets the enumerator for cells in this Range in C++.'
## UnionRange::GetEnumerator method
Gets the enumerator for cells in this [Range](../../range/).
```cpp
Enumerator<Cell> Aspose::Cells::UnionRange::GetEnumerator()
```
## ReturnValue
The cells enumerator
## Remarks
When traversing elements by the returned [Enumerator](../../enumerator/), the cells collection should not be modified(such as operations that will cause new Cell/Row be instantiated or existing Cell/Row be deleted). Otherwise the enumerator may not be able to traverse all cells correctly(some elements may be traversed repeatedly or skipped).
## See Also
* Class [Enumerator](../../enumerator/)
* Class [Cell](../../cell/)
* Class [UnionRange](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
