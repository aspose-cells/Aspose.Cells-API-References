##Aspose::Cells::Row::GetEnumerator method
'Aspose::Cells::Row::GetEnumerator method. Gets the cells enumerator in C++.'
## Row::GetEnumerator() method
Gets the cells enumerator.
```cpp
Enumerator<Cell> Aspose::Cells::Row::GetEnumerator()
```
## ReturnValue
The cells enumerator which will traverse all existing cells in this row.
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook(u"template.xlsx");
Cells cells = workbook.GetWorksheets().Get(0).GetCells();
Enumerator<Cell> en = cells.GetRows().Get(1).GetEnumerator();
while (en.MoveNext())
{
Cell cell = (Cell)en.GetCurrent();
std::cout << cell.GetName().ToUtf8() << std::endl;
}
Aspose::Cells::Cleanup();
```
## See Also
* Class [Enumerator](../../enumerator/)
* Class [Cell](../../cell/)
* Class [Row](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Row::GetEnumerator(bool, bool) method
Gets an enumerator that iterates cells through this row.
```cpp
Enumerator<Cell> Aspose::Cells::Row::GetEnumerator(bool reversed, bool sync)
```
| Parameter | Type | Description |
| --- | --- | --- |
| reversed | bool | whether enumerate cells in reversed order |
| sync | bool | whether the returned enumerator should check the modification of cells in this row and keep synchronized with it. |
## ReturnValue
The cells enumerator which will traverse all existing cells in this row.
## Remarks
If the row will be modified(by operations that may cause new Cell be instantiated or
existing Cell be removed) during the traversal with the enumerator, synchronized enumerator should be used instead of normal enumerator so that the traversal can continue from the position just after the one has been traversed by the last MoveNext(). However, together with the advantage that no element be skipped or traversed repeatedly, the disadvantage for synchronized enumerator is that the performance will be degraded a bit when comparing with normal enumerator.
## See Also
* Class [Enumerator](../../enumerator/)
* Class [Cell](../../cell/)
* Class [Vector](../../vector/)
* Class [Row](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
