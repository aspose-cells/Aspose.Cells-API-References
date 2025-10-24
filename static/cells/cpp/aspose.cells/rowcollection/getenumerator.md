##Aspose::Cells::RowCollection::GetEnumerator method
'Aspose::Cells::RowCollection::GetEnumerator method. Gets an enumerator that iterates rows through this collection in C++.'
## RowCollection::GetEnumerator() method
Gets an enumerator that iterates rows through this collection.
```cpp
Enumerator<Row> Aspose::Cells::RowCollection::GetEnumerator()
```
## ReturnValue
The row enumerator which will traverse all existing rows in this collection.
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook(u"template.xlsx");
Cells cells = workbook.GetWorksheets().Get(0).GetCells();
Enumerator<Row> en = cells.GetRows().GetEnumerator();
while (en.MoveNext())
{
Row row = (Row)en.GetCurrent();
std::cout << row.GetIndex() << ": " << row.GetHeight() << std::endl;
}
Aspose::Cells::Cleanup();
```
## See Also
* Class [Enumerator](../../enumerator/)
* Class [Row](../../row/)
* Class [RowCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## RowCollection::GetEnumerator(bool, bool) method
Gets an enumerator that iterates rows through this collection.
```cpp
Enumerator<Row> Aspose::Cells::RowCollection::GetEnumerator(bool reversed, bool sync)
```
| Parameter | Type | Description |
| --- | --- | --- |
| reversed | bool | whether enumerate rows in reversed order |
| sync | bool | whether the returned enumerator should check the modification of row collection and keep synchronized with it. |
## ReturnValue
The row enumerator which will traverse all existing rows in this collection.
## Remarks
If the row collection will be modified(by operations that may cause new Row be instantiated or
existing Row be removed) during the traversal with the enumerator, synchronized enumerator should be used instead of normal enumerator so that the traversal can continue from the position just after the one has been traversed by the last MoveNext(). However, together with the advantage that no element be skipped or traversed repeatedly, the disadvantage for synchronized enumerator is that the performance will be degraded a bit when comparing with normal enumerator.
## See Also
* Class [Enumerator](../../enumerator/)
* Class [Row](../../row/)
* Class [Vector](../../vector/)
* Class [RowCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
