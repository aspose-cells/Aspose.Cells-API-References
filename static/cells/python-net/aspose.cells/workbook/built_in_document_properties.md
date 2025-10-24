##built_in_document_properties property
## built_in_document_properties property
Returns a [`DocumentProperty`](/cells/python-net/aspose.cells.properties/documentproperty) collection that represents all the built-in document properties of the spreadsheet.
### Remarks
A new property cannot be added to built-in document properties list. You can only get a built-in property and change its value.
The following is the built-in properties name list:
Title
Subject
Author
Keywords
Comments
Template
Last Author
Revision Number
Application Name
Last Print Date
Creation Date
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
Number of Slides
Number of Notes
Number of Hidden Slides
Number of Multimedia Clips
### Example
```python
from aspose.cells import Workbook
workbook = Workbook()
doc = workbook.built_in_document_properties.get("Author")
doc.value = "John Smith"
```
### Definition:
```python
@property
def built_in_document_properties(self):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`BuiltInDocumentPropertyCollection`](/cells/python-net/aspose.cells.properties/builtindocumentpropertycollection)
* class [`DocumentProperty`](/cells/python-net/aspose.cells.properties/documentproperty)
* class [`Workbook`](/cells/python-net/aspose.cells/workbook)
