##Aspose::Cells::PaginatedSaveOptions::SetPageIndex method
'Aspose::Cells::PaginatedSaveOptions::SetPageIndex method. Gets or sets the 0-based index of the first page to save in C++.'
## PaginatedSaveOptions::SetPageIndex method
Gets or sets the 0-based index of the first page to save.
```cpp
void Aspose::Cells::PaginatedSaveOptions::SetPageIndex(int32_t value)
```
## Remarks
Default is 0.
## Examples
```cpp
Aspose::Cells::Startup();
//The following example shows how to render a range of pages (3 and 4) in a Microsoft Excel file to PDF.
//Open an Excel file
Workbook wb(u"Book1.xlsx");
PdfSaveOptions options;
//Print only Page 3 and Page 4 in the output PDF
//Starting page index (0-based index)
if (options.GetPageIndex() != 3)
{
options.SetPageIndex(3);
}
//Number of pages to be printed
if (options.GetPageCount() != 2)
{
options.SetPageCount(2);
}
//Save the PDF file
wb.Save(u"output.pdf", options);
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Class [PaginatedSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
