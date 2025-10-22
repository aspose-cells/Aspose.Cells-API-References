##Aspose::Cells::Range::AutoFill method
'Aspose::Cells::Range::AutoFill method. Automaticall fill the target range in C++.'
## Range::AutoFill(const Range\&) method
Automaticall fill the target range.
```cpp
void Aspose::Cells::Range::AutoFill(const Range &target)
```
| Parameter | Type | Description |
| --- | --- | --- |
| target | const Range\& | the target range. |
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
// Get the first Worksheet Cells.
Cells cells = workbook.GetWorksheets().Get(0).GetCells();
cells.Get(u"A1").PutValue(1);
cells.Get(u"A2").PutValue(2);
Range source = cells.CreateRange(u"A1:A2");
Range targetRange = cells.CreateRange(u"A3:A10");
//fill 3,4,5....10 to the range A3:A10
source.AutoFill(targetRange);
//Save the Excel file
workbook.Save(u"book1.xlsm");
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Class [Range](../)
* Class [Range](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Range::AutoFill(const Range\&, AutoFillType) method
Automaticall fill the target range.
```cpp
void Aspose::Cells::Range::AutoFill(const Range &target, AutoFillType autoFillType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| target | const Range\& | The targed range. |
| autoFillType | AutoFillType | The auto fill type. |
## See Also
* Class [Vector](../../vector/)
* Class [Range](../)
* Enum [AutoFillType](../../autofilltype/)
* Class [Range](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
