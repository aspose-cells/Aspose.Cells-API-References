---
title: set_two_color_gradient méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 40
url: /fr/python-net/aspose.cells.drawing/fillformat/set_two_color_gradient/
is_root: false
---
##  set_two_color_gradient(color1, color2, style, variant) {#aspose.pydrawing.Color-aspose.pydrawing.Color-GradientStyleType-int}
Définit le remplissage spécifié sur un dégradé bicolore.
Ne s'applique qu'à Excel 2007.



```python
def set_two_color_gradient(self, color1, color2, style, variant):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| color1 | aspose.pydrawing.Color | Une couleur dégradée.|
| color2 | aspose.pydrawing.Color | Deux dégradés de couleur.|
| style | [GradientStyleType](/cells/fr/python-net/aspose.cells.drawing/gradientstyletype) | Style d'ombrage dégradé.|
| variant | int |La variante dégradée. Il peut s'agir d'une valeur comprise entre 1 et 4, correspondant à l'une des quatre variantes de l'onglet Dégradé de la boîte de dialogue Effets de remplissage. Si style est GradientStyle.FromCenter, l'argument Variant ne peut être que 1 ou 2.|


##  set_two_color_gradient(color1, transparency1, color2, transparency2, style, variant) {#aspose.pydrawing.Color-float-aspose.pydrawing.Color-float-GradientStyleType-int}
Définit le remplissage spécifié sur un dégradé bicolore.
Ne s'applique qu'à Excel 2007.



```python
def set_two_color_gradient(self, color1, transparency1, color2, transparency2, style, variant):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| color1 | aspose.pydrawing.Color | Une couleur dégradée.|
| transparency1 | float | Le degré de transparence de la couleur1 sous la forme d'une valeur comprise entre 0,0 (opaque) et 1,0 (clair).|
| color2 | aspose.pydrawing.Color | Deux dégradés de couleur.|
| transparency2 | float | Le degré de transparence de la couleur2 sous la forme d'une valeur comprise entre 0,0 (opaque) et 1,0 (clair).|
| style | [GradientStyleType](/cells/fr/python-net/aspose.cells.drawing/gradientstyletype) | Style d'ombrage dégradé.|
| variant | int |La variante dégradée. Il peut s'agir d'une valeur comprise entre 1 et 4, correspondant à l'une des quatre variantes de l'onglet Dégradé de la boîte de dialogue Effets de remplissage. Si style est GradientStyle.FromCenter, l'argument Variant ne peut être que 1 ou 2.|



###  Voir également
* module [aspose.cells.drawing](../../)
* classe [FillFormat](/cells/fr/python-net/aspose.cells.drawing/fillformat)
