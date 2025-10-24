##Aspose::Cells::Cells::GetEnumerator method
'Aspose::Cells::Cells::GetEnumerator method. Gets the cells enumerator in C++.'
## Cells::GetEnumerator method
Gets the cells enumerator.
```cpp
Enumerator<Cell> Aspose::Cells::Cells::GetEnumerator()
```
## ReturnValue
The cells enumerator
## Remarks
When traversing elements by the returned [Enumerator](../../enumerator/), the cells collection should not be modified(such as operations that will cause new Cell/Row be instantiated or existing Cell/Row be deleted). Otherwise the enumerator may not be able to traverse all cells correctly(some elements may be traversed repeatedly or skipped).
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook(u"template.xlsx");
Cells cells = workbook.GetWorksheets().Get(0).GetCells();
Enumerator<Cell> en = cells.GetEnumerator();
while (en.MoveNext())
{
Cell cell = (Cell)en.GetCurrent();
}
Aspose::Cells::Cleanup();
```
## See Also
* Class [Enumerator](../../enumerator/)
* Class [Cell](../../cell/)
* Class [Cells](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
