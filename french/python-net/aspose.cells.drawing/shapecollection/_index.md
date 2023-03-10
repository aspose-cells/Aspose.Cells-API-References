---
title: ShapeCollection classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 530
url: /fr/python-net/aspose.cells.drawing/shapecollection/
is_root: false
---
##  ShapeCollection classe
Représente toute la forme dans une feuille de calcul/un graphique.



Le type ShapeCollection expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [capacity](/cells/fr/python-net/aspose.cells.drawing/shapecollection/capacity) | Obtient ou définit le nombre d'éléments que la liste de tableau peut contenir.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [add_shape_in_chart(type, placement, left, top, right, bottom, image_data)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart/#MsoDrawingType-PlacementType-int-int-int-int-bytes) | Ajouter une forme au graphique. Toutes les unités correspondent à 1/4000 de la zone du graphique.|
| [add_shape_in_chart(type, placement, left, top, right, bottom)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart/#MsoDrawingType-PlacementType-int-int-int-int) | Ajouter une forme au graphique. Toutes les unités correspondent à 1/4000 de la zone du graphique.|
| [add_shape_in_chart_by_scale(type, placement, left, top, right, bottom)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart_by_scale/#MsoDrawingType-PlacementType-float-float-float-float) | Ajouter une forme au graphique. Toutes les unités correspondent à l'échelle en pourcentage de la zone du graphique.|
| [add_shape_in_chart_by_scale(type, placement, left, top, right, bottom, image_data)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart_by_scale/#MsoDrawingType-PlacementType-float-float-float-float-bytes) | Ajouter une forme au graphique. Toutes les unités correspondent à 1/4000 de la zone du graphique.|
| [add_picture(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_picture/#int-int-int-int-io.RawIOBase) | Ajoute une image à la collection.|
| [add_picture(upper_left_row, upper_left_column, stream, width_scale, height_scale)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_picture/#int-int-io.RawIOBase-int-int) | Ajoute une image à la collection.|
| [copy_to(array)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/copy_to/#list) | Copie la totalité de la liste de tableaux dans une liste de tableaux unidimensionnelle compatible, en commençant au début de la liste de tableaux cible.|
| [copy_to(index, array, array_index, count)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/copy_to/#int-list-int-int) |Copie une plage d'éléments de la liste de tableaux vers une liste de tableaux unidimensionnelle compatible, en commençant à l'index spécifié de la liste de tableaux cible.|
| [index_of(item, index)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/index_of/#Shape-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui s'étend de l'index spécifié au dernier élément.|
| [index_of(item, index, count)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/index_of/#Shape-int-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui commence à l'index spécifié et contient le nombre d'éléments spécifié.|
| [last_index_of(item)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/last_index_of/#Shape) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la liste complète du tableau.|
| [last_index_of(item, index)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/last_index_of/#Shape-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui s'étend du premier élément à l'index spécifié.|
| [last_index_of(item, index, count)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/last_index_of/#Shape-int-int) |Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui contient le nombre d'éléments spécifié et se termine à l'index spécifié.|
| [add_copy(source_shape, upper_left_row, top, upper_left_column, left)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_copy/#Shape-int-int-int-int) | Ajoute et copie une forme dans la feuille de calcul.|
| [add_check_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_check_box/#int-int-int-int-int-int) | Ajoute une case à cocher à la feuille de calcul.|
| [add_text_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_text_box/#int-int-int-int-int-int) | Ajoute une zone de texte à la feuille de calcul.|
| [add_spinner(upper_left_row, top, upper_left_column, left, height, width)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_spinner/#int-int-int-int-int-int) | Ajoute un Spinner à la feuille de calcul.|
| [add_scroll_bar(upper_left_row, top, upper_left_column, left, height, width)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_scroll_bar/#int-int-int-int-int-int) | Ajoute un ScrollBar à la feuille de calcul.|
| [add_radio_button(upper_left_row, top, upper_left_column, left, height, width)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_radio_button/#int-int-int-int-int-int) | Ajoute un RadioButton à la feuille de calcul.|
| [add_list_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_list_box/#int-int-int-int-int-int) | Ajoute un ListBox à la feuille de calcul.|
| [add_combo_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_combo_box/#int-int-int-int-int-int) | Ajoute un ComboBox à la feuille de calcul.|
| [add_group_box(upper_left_row, top, upper_left_column, left, height, width)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_group_box/#int-int-int-int-int-int) |Ajoute un GroupBox à la feuille de calcul.|
| [add_button(upper_left_row, top, upper_left_column, left, height, width)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_button/#int-int-int-int-int-int) | Ajoute un bouton à la feuille de calcul.|
| [add_label(upper_left_row, top, upper_left_column, left, height, width)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_label/#int-int-int-int-int-int) | Ajoute une étiquette à la feuille de calcul.|
| [add_label_in_chart(top, left, height, width)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_label_in_chart/#int-int-int-int) | Ajoute une étiquette au graphique.|
| [add_text_box_in_chart(top, left, height, width)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_text_box_in_chart/#int-int-int-int) | Ajoute une zone de texte au graphique.|
| [add_text_effect_in_chart(effect, text, font_name, size, font_bold, font_italic, top, left, height, width)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_text_effect_in_chart/#MsoPresetTextEffect-str-str-int-bool-bool-int-int-int-int) | Insère un objet WordArt dans le graphique|
| [add_text_effect(effect, text, font_name, size, font_bold, font_italic, upper_left_row, top, upper_left_column, left, height, width)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_text_effect/#MsoPresetTextEffect-str-str-int-bool-bool-int-int-int-int-int-int) | Insère un objet WordArt.|
| [add_word_art(style, text, upper_left_row, top, upper_left_column, left, height, width)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_word_art/#PresetWordArtStyle-str-int-int-int-int-int-int) | Ajoute un WordArt prédéfini depuis Excel 2007.s|
| [add_rectangle(upper_left_row, top, upper_left_column, left, height, width)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_rectangle/#int-int-int-int-int-int) | Ajoute un RectangleShape à la feuille de calcul.|
| [add_oval(upper_left_row, top, upper_left_column, left, height, width)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_oval/#int-int-int-int-int-int) | Ajoute un ovale à la feuille de calcul.|
| [add_line(upper_left_row, top, upper_left_column, left, height, width)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_line/#int-int-int-int-int-int) | Ajoute un LineShape à la feuille de calcul.|
| [add_free_floating_shape(type, top, left, height, width, image_data, is_original_size)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_free_floating_shape/#MsoDrawingType-int-int-int-int-bytes-bool) | Ajoute une forme flottante libre à la feuille de calcul. S'applique uniquement à la forme de ligne/d'image.|
| [add_arc(upper_left_row, top, upper_left_column, left, height, width)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_arc/#int-int-int-int-int-int) | Ajoute un ArcShape à la feuille de calcul.|
| [add_shape(type, upper_left_row, top, upper_left_column, left, height, width)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_shape/#MsoDrawingType-int-int-int-int-int-int) | Ajoute une forme à la feuille de calcul.|
| [add_auto_shape(type, upper_left_row, top, upper_left_column, left, height, width)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_auto_shape/#AutoShapeType-int-int-int-int-int-int) | Ajoute une forme automatique à la feuille de calcul.|
| [add_auto_shape_in_chart(type, top, left, height, width)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_auto_shape_in_chart/#AutoShapeType-int-int-int-int) | Ajoute une forme automatique au graphique.|
| [add_active_x_control(type, top_row, top, left_column, left, width, height)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_active_x_control/#aspose.cells.drawing.activexcontrols.ControlType-int-int-int-int-int-int) | Crée un contrôle Activex.|
| [add_svg(upper_left_row, top, upper_left_column, left, height, width, svg_data, compatible_image_data)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_svg/#int-int-int-int-int-int-bytes-bytes) | Ajoute une image svg.|
| [add_icons(upper_left_row, top, upper_left_column, left, height, width, image_byte_data, compatible_image_data)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_icons/#int-int-int-int-int-int-bytes-bytes) | Ajoute une image svg.|
| [add_linked_picture(upper_left_row, upper_left_column, height, width, source_full_name)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_linked_picture/#int-int-int-int-str) | Ajouter une image liée.|
| [add_ole_object_with_linked_image(upper_left_row, upper_left_column, height, width, source_full_name)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_ole_object_with_linked_image/#int-int-int-int-str) | Ajouter une image liée.|
| [add_picture_in_chart(top, left, stream, width_scale, height_scale)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_picture_in_chart/#int-int-io.RawIOBase-int-int) | Ajoute une image au graphique.|
| [add_ole_object(upper_left_row, top, upper_left_column, left, height, width, image_data)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/add_ole_object/#int-int-int-int-int-int-bytes) | Ajoute un OleObject.|
| [copy_comments_in_range(shapes, ca, dest_row, dest_column)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/copy_comments_in_range/#ShapeCollection-CellArea-int-int) | Copiez tous les commentaires de la plage.|
| [copy_in_range(source_shapes, ca, dest_row, dest_column, is_contained)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/copy_in_range/#ShapeCollection-CellArea-int-int-bool) | Copiez les formes de la plage vers la plage de destination.|
| [delete_in_range(ca)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/delete_in_range/#CellArea) | Supprimez les formes de la plage. Les formes de commentaire ne seront pas supprimées.|
| [delete_shape(shape)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/delete_shape/#Shape) |Supprimer une forme. Si la forme fait partie du groupe ou est une forme de commentaire, elle ne sera pas supprimée.|
| [group(group_items)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/group/#list) | Regroupez les formes.|
| [ungroup(group)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/ungroup/#GroupShape) | Dissocie les éléments de forme.|
| [update_selected_value()](/cells/fr/python-net/aspose.cells.drawing/shapecollection/update_selected_value/#) | Mettre à jour la valeur sélectionnée par la valeur de la cellule liée des formes.|
| [binary_search(item)](/cells/fr/python-net/aspose.cells.drawing/shapecollection/binary_search/#Shape) | Recherche un élément dans toute la liste de tableaux triés à l'aide du comparateur par défaut et renvoie l'index de base zéro de l'élément.|



###  Exemple

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# get ShapeCollection
shapes = workbook.worksheets[0].shapes
# do your business
# Save the excel file.
workbook.save("result.xlsx")

```

###  Voir également
* module [aspose.cells.drawing](..)
