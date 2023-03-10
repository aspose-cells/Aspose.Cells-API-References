---
title: classe PdfBookmarkEntry
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 80
url: /it/python-net/aspose.cells.rendering/pdfbookmarkentry/
is_root: false
---
##  classe PdfBookmarkEntry
PdfBookmarkEntry è una voce nel segnalibro pdf.
se la proprietà Text dell'istanza corrente è nulla o "",
l'istanza corrente verrà nascosta e i figli verranno inseriti al livello corrente.



Il tipo PdfBookmarkEntry espone i membri seguenti:

###  Costruttori
| Costruttore| Descrizione|
| :- | :- |
| [PdfBookmarkEntry()](/cells/it/python-net/aspose.cells.rendering/pdfbookmarkentry/__init__/#) | Costruisce una nuova istanza di PdfBookmarkEntry|


###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [text](/cells/it/python-net/aspose.cells.rendering/pdfbookmarkentry/text) | Titolo di un segnalibro.|
| [destination](/cells/it/python-net/aspose.cells.rendering/pdfbookmarkentry/destination) | La cella a cui si collega il segnalibro.|
| [destination_name](/cells/it/python-net/aspose.cells.rendering/pdfbookmarkentry/destination_name) | Ottiene o imposta il nome della destinazione.|
| [sub_entry](/cells/it/python-net/aspose.cells.rendering/pdfbookmarkentry/sub_entry) | Sottovoce di un segnalibro.|
| [is_open](/cells/it/python-net/aspose.cells.rendering/pdfbookmarkentry/is_open) |Quando questa proprietà è vera, il bookmarkentry si espanderà, altrimenti collasserà.|
| [is_collapse](/cells/it/python-net/aspose.cells.rendering/pdfbookmarkentry/is_collapse) | Quando questa proprietà è vera, il bookmarkentry collasserà, altrimenti si espanderà.|



###  Esempio

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

###  Guarda anche
* modulo [aspose.cells.rendering](..)
