---
title: PdfBookmarkEntry classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 80
url: /fr/python-net/aspose.cells.rendering/pdfbookmarkentry/
is_root: false
---
##  PdfBookmarkEntry classe
PdfBookmarkEntry est une entrée dans le signet pdf.
si la propriété Text de l'instance actuelle est nulle ou "",
l'instance actuelle sera masquée et les enfants seront insérés au niveau actuel.



Le type PdfBookmarkEntry expose les membres suivants :

###  Constructeurs
| Constructeur| Description|
| :- | :- |
| [PdfBookmarkEntry()](/cells/fr/python-net/aspose.cells.rendering/pdfbookmarkentry/__init__/#) | Construit une nouvelle instance de PdfBookmarkEntry|


###  Propriétés
| Propriété| Description|
| :- | :- |
| [text](/cells/fr/python-net/aspose.cells.rendering/pdfbookmarkentry/text) | Titre d'un signet.|
| [destination](/cells/fr/python-net/aspose.cells.rendering/pdfbookmarkentry/destination) | La cellule à laquelle le signet est lié.|
| [destination_name](/cells/fr/python-net/aspose.cells.rendering/pdfbookmarkentry/destination_name) | Obtient ou définit le nom de la destination.|
| [sub_entry](/cells/fr/python-net/aspose.cells.rendering/pdfbookmarkentry/sub_entry) | SubEntry d'un signet.|
| [is_open](/cells/fr/python-net/aspose.cells.rendering/pdfbookmarkentry/is_open) |Lorsque cette propriété est vraie, l'entrée de signet se développera, sinon elle se réduira.|
| [is_collapse](/cells/fr/python-net/aspose.cells.rendering/pdfbookmarkentry/is_collapse) | Lorsque cette propriété est vraie, l'entrée de signet s'effondrera, sinon elle se développera.|



###  Exemples

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

###  Voir également
* module [aspose.cells.rendering](..)
