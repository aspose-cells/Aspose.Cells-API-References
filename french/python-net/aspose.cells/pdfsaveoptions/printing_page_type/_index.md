---
title: printing_page_type propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 350
url: /fr/python-net/aspose.cells/pdfsaveoptions/printing_page_type/
is_root: false
---
##  printing_page_type propriété

Indique quelles pages ne seront pas imprimées.

###  Remarques

Si le contenu de la feuille est clairsemé, certaines pages seront totalement vierges dans le fichier pdf de sortie.
Si vous ne voulez pas ces pages vierges, vous pouvez utiliser cette option pour les omettre.

###  Exemple

Le code suivant omet les pages vierges ou les pages qui ne contiennent que du contenu de style comme l'arrière-plan de la cellule, les bordures.

```python
from aspose.cells import PdfSaveOptions, PrintingPageType, Workbook

wb = Workbook("Book1.xlsx")
pdfSaveOptions = PdfSaveOptions()
# ignore blank pages
pdfSaveOptions.printing_page_type = PrintingPageType.IGNORE_BLANK
wb.save("output_ignore_blank_page.pdf", pdfSaveOptions)
# ignore blank pages and pages which only contains some style content like cell background
pdfSaveOptions.printing_page_type = PrintingPageType.IGNORE_STYLE
wb.save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions)

```
###  Définition:
```python
@property
def printing_page_type(self):
    ...
@printing_page_type.setter
def printing_page_type(self, value):
    ...
```

###  Voir également
* module [aspose.cells](../../)
* classe [PdfSaveOptions](/cells/fr/python-net/aspose.cells/pdfsaveoptions)
* classe [PrintingPageType](/cells/fr/python-net/aspose.cells/printingpagetype)
