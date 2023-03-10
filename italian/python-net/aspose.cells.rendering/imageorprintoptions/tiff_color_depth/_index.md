---
title: tiff_color_depth proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 340
url: /it/python-net/aspose.cells.rendering/imageorprintoptions/tiff_color_depth/
is_root: false
---
##  tiff_color_depth proprietà

Ottiene o imposta la profondità di bit da applicare solo quando si salvano le pagine nel formato `Tiff`.

###  Osservazioni

Ha effetto solo quando si salva su TIFF.
Se TiffCompression è impostato su CCITT3, CCITT4, questo non avrà effetto, la profondità di bit dell'immagine tiff generata sarà sempre 1.
###  Definizione:
```python
@property
def tiff_color_depth(self):
    ...
@tiff_color_depth.setter
def tiff_color_depth(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells.rendering](../../)
* classe [ColorDepth](/cells/it/python-net/aspose.cells.rendering/colordepth)
* classe [ImageOrPrintOptions](/cells/it/python-net/aspose.cells.rendering/imageorprintoptions)
