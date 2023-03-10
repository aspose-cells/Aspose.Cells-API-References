---
title: set_preset_color_gradient método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 30
url: /es/python-net/aspose.cells.drawing/fillformat/set_preset_color_gradient/
is_root: false
---
##  set_preset_color_gradient(preset_color, style, variant) {#GradientPresetType-GradientStyleType-int}
Establece el relleno especificado en un degradado de color predeterminado.
Solo aplica para Excel 2007.



```python
def set_preset_color_gradient(self, preset_color, style, variant):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| preset_color | [GradientPresetType](/cells/es/python-net/aspose.cells.drawing/gradientpresettype) | Tipo de color preestablecido|
| style | [GradientStyleType](/cells/es/python-net/aspose.cells.drawing/gradientstyletype) | Estilo de sombreado degradado.|
| variant | int |La variante degradada. Puede ser un valor de 1 a 4, correspondiente a una de las cuatro variantes en la pestaña Degradado en el cuadro de diálogo Efectos de relleno. Si el estilo es GradientStyle.FromCenter, el argumento Variant solo puede ser 1 o 2.|



###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [FillFormat](/cells/es/python-net/aspose.cells.drawing/fillformat)
