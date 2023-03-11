---
title: ImageOrPrintOptions classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 40
url: /fr/python-net/aspose.cells.rendering/imageorprintoptions/
is_root: false
---
##  ImageOrPrintOptions classe
Permet de spécifier des options lors du rendu de la feuille de calcul en images, de l'impression de la feuille de calcul ou du rendu du graphique en image.



Le type ImageOrPrintOptions expose les membres suivants :

###  Constructeurs
| Constructeur| Description|
| :- | :- |
| [ImageOrPrintOptions()](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/__init__/#) | Construit une nouvelle instance de ImageOrPrintOptions|


###  Propriétés
| Propriété| Description|
| :- | :- |
| [save_format](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/save_format) | Obtient ou définit le type de format du fichier de sortie<br/> Assistance Tiff/XPS|
| [print_with_status_dialog](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/print_with_status_dialog) | Si PrintWithStatusDialog = true , une boîte de dialogue affiche l'état d'impression actuel.<br/> sinon, aucune boîte de dialogue de ce type ne s'affichera.|
| [horizontal_resolution](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/horizontal_resolution) | Obtient ou définit la résolution horizontale des images générées, en points par pouce.<br/> Applique la méthode de génération d'image à l'exception des images au format Emf.|
| [vertical_resolution](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/vertical_resolution) | Obtient ou définit la résolution verticale des images générées, en points par pouce.<br/> Applique la méthode de génération d'image à l'exception de l'image au format Emf.|
| [tiff_compression](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/tiff_compression) | Obtient ou définit le type de compression à appliquer uniquement lors de l'enregistrement de pages au format `Tiff`.|
| [tiff_color_depth](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/tiff_color_depth) | Obtient ou définit la profondeur de bits à appliquer uniquement lors de l'enregistrement de pages au format `Tiff`.|
| [printing_page](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/printing_page) | Indique quelles pages ne seront pas imprimées.|
| [quality](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/quality) | Obtient ou définit une valeur déterminant la qualité des images générées<br/>à appliquer uniquement lors de l'enregistrement de pages au format `Jpeg`. La valeur par défaut est 100|
| [image_type](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/image_type) | Obtient ou définit le format des images générées.<br/> valeur par défaut : PNG.|
| [is_cell_auto_fit](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/is_cell_auto_fit) | Indique si la largeur et la hauteur des cellules sont ajustées automatiquement par valeur de cellule.<br/> La valeur par défaut est faux.|
| [one_page_per_sheet](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/one_page_per_sheet) | Si OnePagePerSheet est true , tout le contenu d'une feuille sortira sur une seule page dans le résultat.<br/> Le format de papier de pagesetup sera invalide, et les autres paramètres de pagesetup<br/> prendra toujours effet.|
| [all_columns_in_one_page_per_sheet](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/all_columns_in_one_page_per_sheet) | Si AllColumnsInOnePagePerSheet est true , tout le contenu de la colonne d'une feuille sortira sur une seule page dans le résultat.<br/> La largeur de la taille du papier de pagesetup sera invalide, et les autres paramètres de pagesetup<br/> prendra toujours effet.|
| [draw_object_event_handler](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/draw_object_event_handler) | Implémente cette interface pour obtenir DrawObject et Bound lors du rendu.|
| [chart_image_type](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/chart_image_type) | Indiquez le type d'image du graphique lors de la conversion.<br/> valeur par défaut : PNG.|
| [embeded_image_name_in_svg](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/embeded_image_name_in_svg) | Indiquez le nom de fichier de l'image intégrée en svg.<br/> Cela devrait être un chemin complet avec un répertoire comme "c:\\xpsEmbedded"|
| [svg_fit_to_view_port](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/svg_fit_to_view_port) | si cette propriété est vraie, le svg généré s'adaptera au port d'affichage.|
| [only_area](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/only_area) | Si cette propriété est true , une zone sera générée et aucune échelle ne prendra effet.|
| [text_rendering_hint](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/text_rendering_hint) | Spécifie la qualité du rendu du texte.<br/> La valeur par défaut est TextRenderingHint.SystemDefault|
| [smoothing_mode](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/smoothing_mode) | Spécifie si le lissage (anti-crénelage) est appliqué aux lignes et aux courbes et aux bords des zones remplies.<br/> La valeur par défaut est SmoothingMode.None|
| [transparent](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/transparent) | Indique si le fond de l'image générée doit être transparent.|
| [pixel_format](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/pixel_format) |Obtient ou définit le format de pixel des images générées.|
| [warning_callback](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/warning_callback) | Obtient ou définit un rappel d'avertissement.|
| [page_saving_callback](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/page_saving_callback) | Contrôler/indiquer la progression du processus d'enregistrement de la page.|
| [is_font_substitution_char_granularity](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/is_font_substitution_char_granularity) | Indique s'il faut uniquement remplacer la police de caractère lorsque la police de cellule n'est pas compatible avec celle-ci.|
| [page_index](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/page_index) | Obtient ou définit l'index de base 0 de la première page à enregistrer.|
| [page_count](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/page_count) | Obtient ou définit le nombre de pages à enregistrer.|
| [is_optimized](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/is_optimized) | Indique s'il faut optimiser les éléments de sortie.|
| [default_font](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/default_font) | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule,<br/>Ils peuvent apparaître sous forme de bloc dans pdf, image.<br/>Définissez la police par défaut telle que MingLiu ou MS Gothic pour afficher ces caractères.<br/> Si cette propriété n'est pas définie, Aspose.Cells utilisera la police par défaut du système pour afficher ces caractères Unicode.|
| [check_workbook_default_font](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/check_workbook_default_font) | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule,<br/>Ils peuvent apparaître sous forme de bloc dans pdf, image.<br/> Définissez ceci sur true pour essayer d'utiliser la police par défaut du classeur pour afficher ces caractères en premier.|
| [output_blank_page_when_nothing_to_print](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/output_blank_page_when_nothing_to_print) | Indique s'il faut imprimer une page vierge lorsqu'il n'y a rien à imprimer.|
| [gridline_type](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/gridline_type) | Obtient ou définit le type de quadrillage.|
| [text_cross_type](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/text_cross_type) | Obtient ou définit l'affichage du type de texte lorsque la largeur du texte est supérieure à la largeur de la cellule.|
| [emf_type](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/emf_type) | Obtient ou définit un EmfType qui spécifie le format du métafichier.<br/> La valeur par défaut est EmfPlusDual.|
| [default_edit_language](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/default_edit_language) | Obtient ou définit la langue d'édition par défaut.|
| [sheet_set](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/sheet_set) |Obtient ou définit les feuilles à rendre. La valeur par défaut est toutes les feuilles visibles dans le classeur : [SheetSet.visible](/cells/fr/python-net/aspose.cells.rendering/sheetset#visible).|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [set_desired_size(desired_width, desired_height)](/cells/fr/python-net/aspose.cells.rendering/imageorprintoptions/set_desired_size/#int-int) | Définit la largeur et la hauteur souhaitées de l'image.|



###  Exemple

```python
from aspose.cells import Workbook
from aspose.cells.drawing import ImageType
from aspose.cells.rendering import ImageOrPrintOptions

# Set Image Or Print Options
options = ImageOrPrintOptions()
# Set output image format
options.image_type = ImageType.PNG
# Set Horizontal resolution
options.horizontal_resolution = 300
# Set Vertical Resolution
options.vertical_resolution = 300
# Instantiate Workbook
book = Workbook("test.xls")
# Save chart as Image using ImageOrPrint Options
book.worksheets[0].charts[0].to_image("chart.png", options)

```

###  Voir également
* module [aspose.cells.rendering](..)
