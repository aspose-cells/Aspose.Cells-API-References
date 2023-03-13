---
title: PdfBookmarkEntry Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 80
url: /de/python-net/aspose.cells.rendering/pdfbookmarkentry/
is_root: false
---
##  PdfBookmarkEntry Klasse
PdfBookmarkEntry ist ein Eintrag im PDF-Lesezeichen.
wenn die Text-Eigenschaft der aktuellen Instanz null oder "" ist,
Die aktuelle Instanz wird ausgeblendet und untergeordnete Elemente werden auf der aktuellen Ebene eingefügt.



Der Typ PdfBookmarkEntry macht die folgenden Member verfügbar:

###  Konstrukteure
| Konstrukteur| Beschreibung|
| :- | :- |
| [PdfBookmarkEntry()](/cells/de/python-net/aspose.cells.rendering/pdfbookmarkentry/__init__/#) | Erstellt eine neue Instanz von PdfBookmarkEntry|


###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [text](/cells/de/python-net/aspose.cells.rendering/pdfbookmarkentry/text) | Titel eines Lesezeichens.|
| [destination](/cells/de/python-net/aspose.cells.rendering/pdfbookmarkentry/destination) | Die Zelle, auf die das Lesezeichen verweist.|
| [destination_name](/cells/de/python-net/aspose.cells.rendering/pdfbookmarkentry/destination_name) | Ruft den Namen des Ziels ab oder legt ihn fest.|
| [sub_entry](/cells/de/python-net/aspose.cells.rendering/pdfbookmarkentry/sub_entry) | Untereintrag eines Lesezeichens.|
| [is_open](/cells/de/python-net/aspose.cells.rendering/pdfbookmarkentry/is_open) |Wenn diese Eigenschaft wahr ist, wird die Lesezeichenliste erweitert, andernfalls wird sie zusammenbrechen.|
| [is_collapse](/cells/de/python-net/aspose.cells.rendering/pdfbookmarkentry/is_collapse) | Wenn diese Eigenschaft wahr ist, wird die Lesezeichenliste reduziert, andernfalls wird sie erweitert.|



###  Beispiel

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

###  Siehe auch
* Modul [aspose.cells.rendering](..)
