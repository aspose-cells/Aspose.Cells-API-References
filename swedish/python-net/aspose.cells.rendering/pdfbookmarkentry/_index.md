---
title: PdfBookmarkEntry klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 80
url: /sv/python-net/aspose.cells.rendering/pdfbookmarkentry/
is_root: false
---
##  PdfBookmarkEntry klass
PdfBookmarkEntry är en post i pdf-bokmärke.
om textegenskapen för aktuell instans är null eller "",
aktuell instans kommer att döljas och barn kommer att infogas på aktuell nivå.



Typen PdfBookmarkEntry avslöjar följande medlemmar:

###  Konstruktörer
| Konstruktör| Beskrivning|
| :- | :- |
| [PdfBookmarkEntry()](/cells/sv/python-net/aspose.cells.rendering/pdfbookmarkentry/__init__/#) | Konstruerar en ny instans av PdfBookmarkEntry|


###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [text](/cells/sv/python-net/aspose.cells.rendering/pdfbookmarkentry/text) | Titeln på ett bokmärke.|
| [destination](/cells/sv/python-net/aspose.cells.rendering/pdfbookmarkentry/destination) | Cellen som bokmärket länkar till.|
| [destination_name](/cells/sv/python-net/aspose.cells.rendering/pdfbookmarkentry/destination_name) | Hämtar eller ställer in namnet på destinationen.|
| [sub_entry](/cells/sv/python-net/aspose.cells.rendering/pdfbookmarkentry/sub_entry) | Underpost till ett bokmärke.|
| [is_open](/cells/sv/python-net/aspose.cells.rendering/pdfbookmarkentry/is_open) | När den här egenskapen är sann kommer bokmärkesposten att expandera, annars kommer den att kollapsa.|
| [is_collapse](/cells/sv/python-net/aspose.cells.rendering/pdfbookmarkentry/is_collapse) | När den här egenskapen är sann kommer bokmärkesposten att kollapsa, annars expanderar den.|



###  Exempel

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

###  Se även
* modul [aspose.cells.rendering](..)
