---
title: set_two_color_gradient yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 40
url: /tr/python-net/aspose.cells.drawing/fillformat/set_two_color_gradient/
is_root: false
---
##  set_two_color_gradient(color1, color2, style, variant) {#aspose.pydrawing.Color-aspose.pydrawing.Color-GradientStyleType-int}
Belirtilen dolguyu iki renkli bir degradeye ayarlar.
Yalnızca Excel 2007 için geçerlidir.



```python
def set_two_color_gradient(self, color1, color2, style, variant):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| color1 | aspose.pydrawing.Color | Bir degrade renk.|
| color2 | aspose.pydrawing.Color | İki degrade renk.|
| style | [GradientStyleType](/cells/tr/python-net/aspose.cells.drawing/gradientstyletype) | Degrade gölgeleme stili.|
| variant | int |Gradyan varyantı. Dolgu Efektleri iletişim kutusundaki Degrade sekmesindeki dört değişkenden birine karşılık gelen 1 ile 4 arasında bir değer olabilir. Stil GradientStyle.FromCenter ise, Variant bağımsız değişkeni yalnızca 1 veya 2 olabilir.|


##  set_two_color_gradient(color1, transparency1, color2, transparency2, style, variant) {#aspose.pydrawing.Color-float-aspose.pydrawing.Color-float-GradientStyleType-int}
Belirtilen dolguyu iki renkli bir degradeye ayarlar.
Yalnızca Excel 2007 için geçerlidir.



```python
def set_two_color_gradient(self, color1, transparency1, color2, transparency2, style, variant):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| color1 | aspose.pydrawing.Color | Bir degrade renk.|
| transparency1 | float | 0,0 (opak) ila 1,0 (berrak) arasında bir değer olarak color1'in şeffaflık derecesi.|
| color2 | aspose.pydrawing.Color | İki degrade renk.|
| transparency2 | float | 0,0 (opak) ile 1,0 (berrak) arasında bir değer olarak rengin2 şeffaflık derecesi.|
| style | [GradientStyleType](/cells/tr/python-net/aspose.cells.drawing/gradientstyletype) | Degrade gölgeleme stili.|
| variant | int |Gradyan varyantı. Dolgu Efektleri iletişim kutusundaki Degrade sekmesindeki dört değişkenden birine karşılık gelen 1 ile 4 arasında bir değer olabilir. Stil GradientStyle.FromCenter ise, Variant bağımsız değişkeni yalnızca 1 veya 2 olabilir.|



###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [FillFormat](/cells/tr/python-net/aspose.cells.drawing/fillformat)
