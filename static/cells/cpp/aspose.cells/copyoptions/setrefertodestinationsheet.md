##Aspose::Cells::CopyOptions::SetReferToDestinationSheet method
'Aspose::Cells::CopyOptions::SetReferToDestinationSheet method. When copying the range in the same file and the chart refers to the source sheet, False means the copied chart''s data source will not be changed. True means the copied chart''s data source refers to the destination sheet in C++.'
## CopyOptions::SetReferToDestinationSheet method
When copying the range in the same file and the chart refers to the source sheet, False means the copied chart's data source will not be changed. True means the copied chart's data source refers to the destination sheet.
```cpp
void Aspose::Cells::CopyOptions::SetReferToDestinationSheet(bool value)
```
## Remarks
The default value is false, it works as MS Excel. For example: if copying a chart with the data source "sheet1!A1:B10" from worksheet "sheet1 to other worksheet "sheet2",
The data source will be changed as "sheet2!A1:B10"
## See Also
* Class [Vector](../../vector/)
* Class [CopyOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
