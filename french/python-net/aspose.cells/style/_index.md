---
title: Style classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 1390
url: /fr/python-net/aspose.cells/style/
is_root: false
---
##  Style classe
Représente le style d'affichage du document Excel, tel que la police, la couleur, l'alignement, la bordure, etc.
L'objet Style contient tous les attributs de style (police, format de nombre, alignement, etc.) en tant que propriétés.



Le type Style expose les membres suivants :

###  Constructeurs
| Constructeur| Description|
| :- | :- |
| [Style()](/cells/fr/python-net/aspose.cells/style/__init__/#) | Initialise une nouvelle instance de la classe [Style](/cells/fr/python-net/aspose.cells/style).|


###  Propriétés
| Propriété| Description|
| :- | :- |
| [background_theme_color](/cells/fr/python-net/aspose.cells/style/background_theme_color) | Obtient et définit la couleur du thème d'arrière-plan.|
| [foreground_theme_color](/cells/fr/python-net/aspose.cells/style/foreground_theme_color) | Obtient et définit la couleur du thème de premier plan.|
| [name](/cells/fr/python-net/aspose.cells/style/name) | Obtient ou définit le nom du style.|
| [pattern](/cells/fr/python-net/aspose.cells/style/pattern) |Obtient ou définit le type de motif d'arrière-plan de la cellule.|
| [borders](/cells/fr/python-net/aspose.cells/style/borders) | Obtient le [BorderCollection](/cells/fr/python-net/aspose.cells/bordercollection) du style.|
| [background_color](/cells/fr/python-net/aspose.cells/style/background_color) | Obtient ou définit la couleur d'arrière-plan d'un style.|
| [background_argb_color](/cells/fr/python-net/aspose.cells/style/background_argb_color) | Obtient et définit la couleur d'arrière-plan avec une valeur ARGB 32 bits.|
| [foreground_color](/cells/fr/python-net/aspose.cells/style/foreground_color) | Obtient ou définit la couleur de premier plan d'un style.|
| [foreground_argb_color](/cells/fr/python-net/aspose.cells/style/foreground_argb_color) | Obtient et définit la couleur de premier plan avec une valeur ARGB 32 bits.|
| [has_borders](/cells/fr/python-net/aspose.cells/style/has_borders) | Vérifie si des bordures ont été définies pour le style.|
| [parent_style](/cells/fr/python-net/aspose.cells/style/parent_style) | Obtient le style parent de ce style.|
| [indent_level](/cells/fr/python-net/aspose.cells/style/indent_level) | Représente le niveau de retrait de la cellule ou de la plage.|
| [font](/cells/fr/python-net/aspose.cells/style/font) | Obtient un objet [Style.font](/cells/fr/python-net/aspose.cells/style#font).|
| [rotation_angle](/cells/fr/python-net/aspose.cells/style/rotation_angle) | Représente l'angle de rotation du texte.|
| [horizontal_alignment](/cells/fr/python-net/aspose.cells/style/horizontal_alignment) | Obtient ou définit le type d'alignement horizontal du texte dans une cellule.|
| [vertical_alignment](/cells/fr/python-net/aspose.cells/style/vertical_alignment) | Obtient ou définit le type d'alignement vertical du texte dans une cellule.|
| [is_text_wrapped](/cells/fr/python-net/aspose.cells/style/is_text_wrapped) | Obtient ou définit une valeur indiquant si le texte d'une cellule est renvoyé à la ligne.|
| [number](/cells/fr/python-net/aspose.cells/style/number) | Obtient ou définit le format d'affichage des nombres et des dates.|
| [is_locked](/cells/fr/python-net/aspose.cells/style/is_locked) |Obtient ou définit une valeur indiquant si une cellule peut être modifiée ou non.|
| [custom](/cells/fr/python-net/aspose.cells/style/custom) | Représente la chaîne de format de nombre personnalisé de cet objet de style.<br/> Si le format numérique personnalisé n'est pas défini (par exemple, le format numérique est intégré), "" sera renvoyé.|
| [culture_custom](/cells/fr/python-net/aspose.cells/style/culture_custom) | Obtient et définit la chaîne de modèle dépendante de la culture pour le format numérique.<br/>Si aucun format de nombre n'a été défini pour cet objet, null sera renvoyé.<br/> Si le format de nombre est intégré, la chaîne de modèle correspondant au nombre intégré sera renvoyée.|
| [invariant_custom](/cells/fr/python-net/aspose.cells/style/invariant_custom) | Obtient la chaîne de modèle indépendante de la culture pour le format numérique.<br/>Si aucun format de nombre n'a été défini pour cet objet, null sera renvoyé.<br/> Si le format de nombre est intégré, la chaîne de modèle correspondant au nombre intégré sera renvoyée.|
| [is_formula_hidden](/cells/fr/python-net/aspose.cells/style/is_formula_hidden) | Représente si la formule sera masquée lorsque la feuille de calcul est protégée.|
| [shrink_to_fit](/cells/fr/python-net/aspose.cells/style/shrink_to_fit) | Représente si le texte est automatiquement réduit pour tenir dans la largeur de colonne disponible.|
| [text_direction](/cells/fr/python-net/aspose.cells/style/text_direction) | Représente l'ordre de lecture du texte.|
| [is_justify_distributed](/cells/fr/python-net/aspose.cells/style/is_justify_distributed) | Indique si l'alignement justifié ou distribué des cellules doit être utilisé sur la dernière ligne de texte.|
| [quote_prefix](/cells/fr/python-net/aspose.cells/style/quote_prefix) | Indique si la valeur de la cellule commence par un guillemet simple.|
| [is_gradient](/cells/fr/python-net/aspose.cells/style/is_gradient) | Indique si l'ombrage des cellules est un motif dégradé.|
| [is_percent](/cells/fr/python-net/aspose.cells/style/is_percent) |Indique si le format numérique est un format de pourcentage.|
| [is_date_time](/cells/fr/python-net/aspose.cells/style/is_date_time) | Indique si le format numérique est un format de date.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [set_border(border_type, border_style, border_color)](/cells/fr/python-net/aspose.cells/style/set_border/#BorderType-CellBorderType-aspose.pydrawing.Color) | Définit les bordures du style.|
| [set_border(border_type, border_style, border_color)](/cells/fr/python-net/aspose.cells/style/set_border/#BorderType-CellBorderType-CellsColor) | Définit les bordures du style.|
| [set_pattern_color(pattern, color1, color2)](/cells/fr/python-net/aspose.cells/style/set_pattern_color/#BackgroundType-aspose.pydrawing.Color-aspose.pydrawing.Color) | Définit la couleur d'arrière-plan.|
| [copy(style)](/cells/fr/python-net/aspose.cells/style/copy/#Style) | Copie les données d'un autre objet de style|
| [update()](/cells/fr/python-net/aspose.cells/style/update/#) | Appliquez le style nommé aux styles des cellules qui utilisent ce style nommé.<br/>Cela fonctionne comme si vous cliquiez sur le bouton "ok" après avoir fini de modifier le style.<br/> Ne s'applique qu'au style nommé.|
| [is_modified(modify_flag)](/cells/fr/python-net/aspose.cells/style/is_modified/#StyleModifyFlag) | Vérifie si les propriétés spécifiées du style ont été modifiées.<br/> Utilisé pour le style de ConditionalFormattings pour vérifier si les propriétés spécifiées de ce style doivent être utilisées lors de l'application de ConditionalFormattings sur une cellule.|
| [set_custom(custom, builtin_preference)](/cells/fr/python-net/aspose.cells/style/set_custom/#str-bool) | Définit la chaîne de format numérique personnalisé d'une cellule.|
| [set_two_color_gradient(color1, color2, gradient_style_type, variant)](/cells/fr/python-net/aspose.cells/style/set_two_color_gradient/#aspose.pydrawing.Color-aspose.pydrawing.Color-aspose.cells.drawing.GradientStyleType-int) | Définit le remplissage spécifié sur un dégradé bicolore.|
| [get_two_color_gradient(color1, color2, gradient_style_type, variant)](/cells/fr/python-net/aspose.cells/style/get_two_color_gradient/#aspose.pydrawing.Color&-aspose.pydrawing.Color&-any-any) | Obtenez le paramètre de dégradé bicolore.|
| [get_two_color_gradient_setting()](/cells/fr/python-net/aspose.cells/style/get_two_color_gradient_setting/#) | Obtenez le paramètre de dégradé bicolore.|
| [to_json()](/cells/fr/python-net/aspose.cells/style/to_json/#) | Convertissez les données de structure [Style](/cells/fr/python-net/aspose.cells/style) en JSON.|



###  Exemples

```python
from aspose.cells import Workbook
from aspose.pydrawing import Color

workbook = Workbook()
sheets = workbook.worksheets
cell = sheets[0].cells.get("A1")
style = cell.get_style()
style.font.name = "Times New Roman"
style.font.color = Color.blue
cell.set_style(style)

```

###  Voir également
* module [aspose.cells](..)
* classe [BorderCollection](/cells/fr/python-net/aspose.cells/bordercollection)
* classe [Style](/cells/fr/python-net/aspose.cells/style)
