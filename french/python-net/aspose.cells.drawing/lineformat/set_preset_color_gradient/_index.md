---
title: set_preset_color_gradient méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 30
url: /fr/python-net/aspose.cells.drawing/lineformat/set_preset_color_gradient/
is_root: false
---
##  set_preset_color_gradient(preset_color, style, variant) {#GradientPresetType-GradientStyleType-int}
Définit le remplissage spécifié sur un dégradé de couleur prédéfini.
Ne s'applique qu'à Excel 2007.



```python
def set_preset_color_gradient(self, preset_color, style, variant):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| preset_color | [GradientPresetType](/cells/fr/python-net/aspose.cells.drawing/gradientpresettype) | Type de couleur prédéfini|
| style | [GradientStyleType](/cells/fr/python-net/aspose.cells.drawing/gradientstyletype) | Style d'ombrage dégradé.|
| variant | int |La variante dégradée. Il peut s'agir d'une valeur comprise entre 1 et 4, correspondant à l'une des quatre variantes de l'onglet Dégradé de la boîte de dialogue Effets de remplissage. Si style est GradientStyle.FromCenter, l'argument Variant ne peut être que 1 ou 2.|



###  Voir également
* module [aspose.cells.drawing](../../)
* classe [LineFormat](/cells/fr/python-net/aspose.cells.drawing/lineformat)
