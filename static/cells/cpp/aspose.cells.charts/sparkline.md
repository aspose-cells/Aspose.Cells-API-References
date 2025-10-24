##Aspose::Cells::Charts::Sparkline class
'Aspose::Cells::Charts::Sparkline class. A sparkline represents a tiny chart or graphic in a worksheet cell that provides a visual representation of data in C++.'
## Sparkline class
A sparkline represents a tiny chart or graphic in a worksheet cell that provides a visual representation of data.
```cpp
class Sparkline
```
## Methods
| Method | Description |
| --- | --- |
| [GetColumn()](./getcolumn/) | Gets the column index of the sparkline. |
| [GetDataRange()](./getdatarange/) | Represents the data range of the sparkline. |
| [GetRow()](./getrow/) | Gets the row index of the sparkline. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Sparkline\& src)](./operator_asm/) | operator= |
| [SetDataRange(const U16String\& value)](./setdatarange/) | Represents the data range of the sparkline. |
| [SetDataRange(const char16_t* value)](./setdatarange/) | Represents the data range of the sparkline. |
| [Sparkline(Sparkline_Impl* impl)](./sparkline/) | Constructs from an implementation object. |
| [Sparkline(const Sparkline\& src)](./sparkline/) | Copy constructor. |
| [ToImage(const U16String\& fileName, const ImageOrPrintOptions\& options)](./toimage/) | Converts a sparkline to an image. |
| [ToImage(const char16_t* fileName, const ImageOrPrintOptions\& options)](./toimage/) | Converts a sparkline to an image. |
| [ToImage(const ImageOrPrintOptions\& options)](./toimage/) | Converts a sparkline to an image. |
| [~Sparkline()](./~sparkline/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook book;
Worksheet sheet = book.GetWorksheets().Get(0);
sheet.GetCells().Get(u"A1").PutValue(5);
sheet.GetCells().Get(u"B1").PutValue(2);
sheet.GetCells().Get(u"C1").PutValue(1);
sheet.GetCells().Get(u"D1").PutValue(3);
// Define the CellArea
CellArea ca;
ca.StartColumn = 4;
ca.EndColumn = 4;
ca.StartRow = 0;
ca.EndRow = 0;
int idx = sheet.GetSparklineGroups().Add(SparklineType::Line, sheet.GetName() + u"!A1:D1", false, ca);
SparklineGroup group = sheet.GetSparklineGroups().Get(idx);
idx = group.GetSparklines().Add(sheet.GetName() + u"!A1:D1", 0, 4);
Sparkline line = group.GetSparklines().Get(idx);
std::cout << "Saprkline data range: " << line.GetDataRange().ToUtf8() << ", row: " << line.GetRow() << ", column: " << line.GetColumn() <<std::endl;
line.ToImage(u"output.png", ImageOrPrintOptions());
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::Charts](../)
* Library [Aspose.Cells for C++](../../)
