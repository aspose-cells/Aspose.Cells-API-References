##Aspose::Cells::Workbook::GetCustomDocumentProperties method
'Aspose::Cells::Workbook::GetCustomDocumentProperties method. Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet in C++.'
## Workbook::GetCustomDocumentProperties method
Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet.
```cpp
CustomDocumentPropertyCollection Aspose::Cells::Workbook::GetCustomDocumentProperties()
```
## Examples
```cpp
Aspose::Cells::Startup();
Workbook excel;
excel.GetCustomDocumentProperties().Add(u"Checked by", u"Jane");
Aspose::Cells::Cleanup();
```
## See Also
* Class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
