---
title: page_index propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 190
url: /fr/python-net/aspose.cells/xpssaveoptions/page_index/
is_root: false
---
##  page_index propriété

Obtient ou définit l'index de base 0 de la première page à enregistrer.

###  Remarques

La valeur par défaut est 0.

###  Exemple

L'exemple suivant montre comment rendre une plage de pages (3 et 4) dans un fichier Excel Microsoft en PDF.

```python
from aspose.cells import PdfSaveOptions, Workbook

# Open an Excel file
wb = Workbook("Book1.xlsx")
options = PdfSaveOptions()
# Print only Page 3 and Page 4 in the output PDF
# Starting page index (0-based index)
options.page_index = 3
# Number of pages to be printed
options.page_count = 2
# Save the PDF file
wb.save("output.pdf", options)

```
###  Définition:
```python
@property
def page_index(self):
    ...
@page_index.setter
def page_index(self, value):
    ...
```

###  Voir également
* module [aspose.cells](../../)
* classe [XpsSaveOptions](/cells/fr/python-net/aspose.cells/xpssaveoptions)
