---
title: trim_tailing_blank_cells propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 230
url: /es/python-net/aspose.cells/txtsaveoptions/trim_tailing_blank_cells/
is_root: false
---
##  trim_tailing_blank_cells propiedad

Indica si se deben recortar las celdas en blanco de cola en una fila. El valor predeterminado es falso.

###  Observaciones

Al guardar con el modo LightCells y no se ha especificado el [TxtSaveOptions.export_area](/cells/es/python-net/aspose.cells/txtsaveoptions#export_area),
esta opción no tiene efecto y una fila se extenderá hasta la última celda proporcionada por
la implementación [TxtSaveOptions.light_cells_data_provider](/cells/es/python-net/aspose.cells/txtsaveoptions#light_cells_data_provider)
###  Definición:
```python
@property
def trim_tailing_blank_cells(self):
    ...
@trim_tailing_blank_cells.setter
def trim_tailing_blank_cells(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells](../../)
* clase [TxtSaveOptions](/cells/es/python-net/aspose.cells/txtsaveoptions)
