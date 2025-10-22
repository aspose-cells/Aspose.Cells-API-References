##Aspose::Cells::Range::Intersect method
'Aspose::Cells::Range::Intersect method. Returns a Range object that represents the rectangular intersection of two ranges in C++.'
## Range::Intersect method
Returns a [Range](../) object that represents the rectangular intersection of two ranges.
```cpp
Range Aspose::Cells::Range::Intersect(const Range &range)
```
| Parameter | Type | Description |
| --- | --- | --- |
| range | const Range\& | The intersecting range. |
## ReturnValue
Returns a [Range](../) object
## Remarks
If the two ranges are not intersected, returns null.
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
// Get the first Worksheet Cells.
Cells cells = workbook.GetWorksheets().Get(0).GetCells();
Range range1 = cells.CreateRange(u"A1:A5");
Range range2 = cells.CreateRange(u"A3:A10");
//Get intersected range of the two ranges.
Range intersectRange = range1.Intersect(range2);
//Save the Excel file
workbook.Save(u"book1.xlsm");
Aspose::Cells::Cleanup();
```
## See Also
* Class [Range](../)
* Class [Vector](../../vector/)
* Class [Range](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
