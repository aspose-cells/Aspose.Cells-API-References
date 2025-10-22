##PdfBookmarkEntry class
## PdfBookmarkEntry class
PdfBookmarkEntry is an entry in pdf bookmark.
if Text property of current instance is null or "",
current instance will be hidden and children will be inserted on current level.
The PdfBookmarkEntry type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self)`](/cells/python-net/aspose.cells.rendering/pdfbookmarkentry/__init__/#) | Constructs a new instance of PdfBookmarkEntry |
### Properties
| Property | Description |
| :- | :- |
| [text](/cells/python-net/aspose.cells.rendering/pdfbookmarkentry/text) | Title of a bookmark. |
| [destination](/cells/python-net/aspose.cells.rendering/pdfbookmarkentry/destination) | The cell to which the bookmark link. |
| [destination_name](/cells/python-net/aspose.cells.rendering/pdfbookmarkentry/destination_name) | Gets or sets name of destination. |
| [sub_entry](/cells/python-net/aspose.cells.rendering/pdfbookmarkentry/sub_entry) | SubEntry of a bookmark. |
| [is_open](/cells/python-net/aspose.cells.rendering/pdfbookmarkentry/is_open) | When this property is true, the bookmarkentry will expand, otherwise it will collapse. |
| [is_collapse](/cells/python-net/aspose.cells.rendering/pdfbookmarkentry/is_collapse) | When this property is true, the bookmarkentry will collapse, otherwise it will expand. |
### Example
```python
from aspose.cells import PdfSaveOptions, Workbook
from aspose.cells.rendering import PdfBookmarkEntry
workbook = Workbook()
workbook.worksheets.add()
workbook.worksheets.add()
cellInPage1 = workbook.worksheets[0].cells.get("A1")
cellInPage2 = workbook.worksheets[1].cells.get("A1")
cellInPage3 = workbook.worksheets[2].cells.get("A1")
cellInPage1.put_value("page1")
cellInPage2.put_value("page2")
cellInPage3.put_value("page3")
pbeRoot = PdfBookmarkEntry()
pbeRoot.text = "root"
pbeRoot.destination = cellInPage1
pbeRoot.sub_entry = []
pbeRoot.is_open = False
subPbe1 = PdfBookmarkEntry()
subPbe1.text = "section1"
subPbe1.destination = cellInPage2
subPbe2 = PdfBookmarkEntry()
subPbe2.text = "section2"
subPbe2.destination = cellInPage3
pbeRoot.sub_entry.append(subPbe1)
pbeRoot.sub_entry.append(subPbe2)
saveOptions = PdfSaveOptions()
saveOptions.bookmark = pbeRoot
workbook.save("output_bookmark.pdf", saveOptions)
```
### See Also
* module [`aspose.cells.rendering`](..)
