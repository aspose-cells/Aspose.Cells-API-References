---
title: metodo set_two_color_gradient
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 40
url: /it/python-net/aspose.cells.drawing/fillformat/set_two_color_gradient/
is_root: false
---
##  set_two_color_gradient(color1, color2, style, variant) {#aspose.pydrawing.Color-aspose.pydrawing.Color-GradientStyleType-int}
Imposta il riempimento specificato su una sfumatura a due colori.
Si applica solo a Excel 2007.



```python
def set_two_color_gradient(self, color1, color2, style, variant):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| color1 | aspose.pydrawing.Color | Un colore sfumato.|
| color2 | aspose.pydrawing.Color | Due colori sfumati.|
| style | [GradientStyleType](/cells/it/python-net/aspose.cells.drawing/gradientstyletype) | Stile di sfumatura sfumata.|
| variant | int |La variante gradiente. Può essere un valore compreso tra 1 e 4, corrispondente a una delle quattro varianti nella scheda Sfumatura nella finestra di dialogo Effetti di riempimento. Se style è GradientStyle.FromCenter, l'argomento Variant può essere solo 1 o 2.|


##  set_two_color_gradient(color1, transparency1, color2, transparency2, style, variant) {#aspose.pydrawing.Color-float-aspose.pydrawing.Color-float-GradientStyleType-int}
Imposta il riempimento specificato su una sfumatura a due colori.
Si applica solo a Excel 2007.



```python
def set_two_color_gradient(self, color1, transparency1, color2, transparency2, style, variant):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| color1 | aspose.pydrawing.Color | Un colore sfumato.|
| transparency1 | float | Il grado di trasparenza del colore1 come valore compreso tra 0,0 (opaco) e 1,0 (trasparente).|
| color2 | aspose.pydrawing.Color | Due colori sfumati.|
| transparency2 | float | Il grado di trasparenza del colore2 come valore compreso tra 0,0 (opaco) e 1,0 (trasparente).|
| style | [GradientStyleType](/cells/it/python-net/aspose.cells.drawing/gradientstyletype) | Stile di sfumatura sfumata.|
| variant | int |La variante gradiente. Può essere un valore compreso tra 1 e 4, corrispondente a una delle quattro varianti nella scheda Sfumatura nella finestra di dialogo Effetti di riempimento. Se style è GradientStyle.FromCenter, l'argomento Variant può essere solo 1 o 2.|



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [FillFormat](/cells/it/python-net/aspose.cells.drawing/fillformat)
