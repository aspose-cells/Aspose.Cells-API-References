---
title: trim_leading_blank_row_and_column fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 220
url: /sv/python-net/aspose.cells/txtsaveoptions/trim_leading_blank_row_and_column/
is_root: false
---
##  trim_leading_blank_row_and_column fastighet

Indikerar om inledande tomma rader och kolumner ska trimmas som vad ms excel gör.
Standard är sant.

###  Anmärkningar

Samma med regeln i ms excel, en rad/kolumn tas inte som tom om den har anpassad stil,
även om den inte innehåller några celldata.
När du sparar med LightCells-läge har det här alternativet ingen effekt.
Användaren bör kontrollera utdataområdet genom att implementera [TxtSaveOptions.light_cells_data_provider](/cells/sv/python-net/aspose.cells/txtsaveoptions#light_cells_data_provider)
eller genom att ange [TxtSaveOptions.export_area](/cells/sv/python-net/aspose.cells/txtsaveoptions#export_area)
###  Definition:
```python
@property
def trim_leading_blank_row_and_column(self):
    ...
@trim_leading_blank_row_and_column.setter
def trim_leading_blank_row_and_column(self, value):
    ...
```

###  Se även
* modul [aspose.cells](../../)
* klass [TxtSaveOptions](/cells/sv/python-net/aspose.cells/txtsaveoptions)
