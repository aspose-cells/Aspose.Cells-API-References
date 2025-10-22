##Aspose::Cells::WorksheetCollection::GetCustomDocumentProperties method
'Aspose::Cells::WorksheetCollection::GetCustomDocumentProperties method. Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet in C++.'
## WorksheetCollection::GetCustomDocumentProperties method
Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet.
```cpp
CustomDocumentPropertyCollection Aspose::Cells::WorksheetCollection::GetCustomDocumentProperties()
```
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
workbook.GetWorksheets().GetCustomDocumentProperties().Add(u"Checked by", u"Jane");
Aspose::Cells::Cleanup();
```
## See Also
* Class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* Class [WorksheetCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
