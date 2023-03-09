---
title: tiff_color_depth propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 340
url: /fr/python-net/aspose.cells.rendering/imageorprintoptions/tiff_color_depth/
is_root: false
---
##  tiff_color_depth propriété

Obtient ou définit la profondeur de bits à appliquer uniquement lors de l'enregistrement de pages au format `Tiff`.

###  Remarques

N'a d'effet que lors de l'enregistrement au TIFF.
Si TiffCompression est défini sur CCITT3, CCITT4, cela ne prendra pas effet, la profondeur de bits de l'image tiff générée sera toujours 1.
###  Définition:
```python
@property
def tiff_color_depth(self):
    ...
@tiff_color_depth.setter
def tiff_color_depth(self, value):
    ...
```

###  Voir également
* module [aspose.cells.rendering](../../)
* classe [ColorDepth](/cells/fr/python-net/aspose.cells.rendering/colordepth)
* classe [ImageOrPrintOptions](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions)
