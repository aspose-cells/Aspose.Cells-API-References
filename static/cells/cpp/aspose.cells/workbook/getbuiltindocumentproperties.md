##Aspose::Cells::Workbook::GetBuiltInDocumentProperties method
'Aspose::Cells::Workbook::GetBuiltInDocumentProperties method. Returns a DocumentProperty collection that represents all the built-in document properties of the spreadsheet in C++.'
## Workbook::GetBuiltInDocumentProperties method
Returns a DocumentProperty collection that represents all the built-in document properties of the spreadsheet.
```cpp
BuiltInDocumentPropertyCollection Aspose::Cells::Workbook::GetBuiltInDocumentProperties()
```
## Remarks
A new property cannot be added to built-in document properties list. You can only get a built-in property and change its value. The following is the built-in properties name list:
Title
Subject
Author
Keywords
Comments
Template
Last Author
Revision Number
Application [Name](../../name/)
Last Print [Date](../../date/)
Creation [Date](../../date/)
Last Save Time
Total Editing Time
Number of Pages
Number of Words
Number of Characters
Security
Category
Format
Manager
Company
Number of Bytes
Number of Lines
Number of Paragraphs
Number of [Slides](../../../aspose.cells.slides/)
Number of Notes
Number of Hidden [Slides](../../../aspose.cells.slides/)
Number of Multimedia Clips
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
DocumentProperty doc = workbook.GetBuiltInDocumentProperties().Get(u"Author");
Aspose::Cells::Cleanup();
```
## See Also
* Class [BuiltInDocumentPropertyCollection](../../../aspose.cells.properties/builtindocumentpropertycollection/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
