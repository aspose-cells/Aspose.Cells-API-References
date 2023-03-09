---
title: PaginatedSaveOptions classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 1150
url: /fr/python-net/aspose.cells/paginatedsaveoptions/
is_root: false
---
##  PaginatedSaveOptions classe
Représente les options de pagination.



**Héritage:** [PaginatedSaveOptions](/cells/python-net/aspose.cells/paginatedsaveoptions) → 
[SaveOptions](/cells/fr/python-net/aspose.cells/saveoptions)



Le type PaginatedSaveOptions expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [save_format](/cells/fr/python-net/aspose.cells/paginatedsaveoptions/save_format) | Obtient le format du fichier de sauvegarde.|
| [clear_data](/cells/fr/python-net/aspose.cells/paginatedsaveoptions/clear_data) | Videz le classeur après avoir enregistré le fichier.|
| [cached_file_folder](/cells/fr/python-net/aspose.cells/paginatedsaveoptions/cached_file_folder) | Le dossier de fichiers mis en cache est utilisé pour stocker des données volumineuses.|
| [validate_merged_areas](/cells/fr/python-net/aspose.cells/paginatedsaveoptions/validate_merged_areas) | Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier.|
| [merge_areas](/cells/fr/python-net/aspose.cells/paginatedsaveoptions/merge_areas) | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier.|
| [create_directory](/cells/fr/python-net/aspose.cells/paginatedsaveoptions/create_directory) | Si true et que le répertoire n'existe pas, le répertoire sera automatiquement créé avant d'enregistrer le fichier.|
| [sort_names](/cells/fr/python-net/aspose.cells/paginatedsaveoptions/sort_names) | Indique s'il faut trier les noms définis avant d'enregistrer le fichier.|
| [sort_external_names](/cells/fr/python-net/aspose.cells/paginatedsaveoptions/sort_external_names) | Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier.|
| [refresh_chart_cache](/cells/fr/python-net/aspose.cells/paginatedsaveoptions/refresh_chart_cache) |Indique si l'actualisation des données du cache du graphique|
| [warning_callback](/cells/fr/python-net/aspose.cells/paginatedsaveoptions/warning_callback) | Obtient ou définit un rappel d'avertissement.|
| [update_smart_art](/cells/fr/python-net/aspose.cells/paginatedsaveoptions/update_smart_art) | Indique si la mise à jour du paramètre d'art intelligent.<br/> La valeur par défaut est faux.|
| [default_font](/cells/fr/python-net/aspose.cells/paginatedsaveoptions/default_font) | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule,<br/>Ils peuvent apparaître sous forme de bloc dans pdf, image.<br/>Définissez la police par défaut telle que MingLiu ou MS Gothic pour afficher ces caractères.<br/> Si cette propriété n'est pas définie, Aspose.Cells utilisera la police par défaut du système pour afficher ces caractères Unicode.|
| [check_workbook_default_font](/cells/fr/python-net/aspose.cells/paginatedsaveoptions/check_workbook_default_font) | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule,<br/>Ils peuvent apparaître sous forme de bloc dans pdf, image.<br/> Définissez ceci sur true pour essayer d'utiliser la police par défaut du classeur pour afficher ces caractères en premier.|
| [check_font_compatibility](/cells/fr/python-net/aspose.cells/paginatedsaveoptions/check_font_compatibility) | Indique s'il faut vérifier la compatibilité des polices pour chaque caractère du texte.|
| [is_font_substitution_char_granularity](/cells/fr/python-net/aspose.cells/paginatedsaveoptions/is_font_substitution_char_granularity) | Indique s'il faut uniquement remplacer la police de caractère lorsque la police de cellule n'est pas compatible avec celle-ci.|
| [one_page_per_sheet](/cells/fr/python-net/aspose.cells/paginatedsaveoptions/one_page_per_sheet) | Si OnePagePerSheet est true , tout le contenu d'une feuille sortira sur une seule page dans le résultat.<br/> Le format de papier de pagesetup sera invalide, et les autres paramètres de pagesetup<br/> prendra toujours effet.|
| [all_columns_in_one_page_per_sheet](/cells/fr/python-net/aspose.cells/paginatedsaveoptions/all_columns_in_one_page_per_sheet) | Si AllColumnsInOnePagePerSheet est true , tout le contenu de la colonne d'une feuille sortira sur une seule page dans le résultat.<br/> La largeur de la taille du papier de pagesetup sera ignorée, et les autres paramètres de pagesetup<br/> prendra toujours effet.|
| [ignore_error](/cells/fr/python-net/aspose.cells/paginatedsaveoptions/ignore_error) | Indique si vous devez masquer l'erreur lors du rendu.<br/> L'erreur peut être une erreur de forme, d'image, de rendu graphique, etc.|
| [output_blank_page_when_nothing_to_print](/cells/fr/python-net/aspose.cells/paginatedsaveoptions/output_blank_page_when_nothing_to_print) | Indique s'il faut imprimer une page vierge lorsqu'il n'y a rien à imprimer.|
| [page_index](/cells/fr/python-net/aspose.cells/paginatedsaveoptions/page_index) | Obtient ou définit l'index de base 0 de la première page à enregistrer.|
| [page_count](/cells/fr/python-net/aspose.cells/paginatedsaveoptions/page_count) | Obtient ou définit le nombre de pages à enregistrer.|
| [printing_page_type](/cells/fr/python-net/aspose.cells/paginatedsaveoptions/printing_page_type) | Indique quelles pages ne seront pas imprimées.|
| [gridline_type](/cells/fr/python-net/aspose.cells/paginatedsaveoptions/gridline_type) | Obtient ou définit le type de quadrillage.|
| [text_cross_type](/cells/fr/python-net/aspose.cells/paginatedsaveoptions/text_cross_type) | Obtient ou définit l'affichage du type de texte lorsque la largeur du texte est supérieure à la largeur de la cellule.|
| [default_edit_language](/cells/fr/python-net/aspose.cells/paginatedsaveoptions/default_edit_language) | Obtient ou définit la langue d'édition par défaut.|
| [sheet_set](/cells/fr/python-net/aspose.cells/paginatedsaveoptions/sheet_set) |Obtient ou définit les feuilles à rendre. La valeur par défaut est toutes les feuilles visibles dans le classeur : [SheetSet.visible](/cells/fr/python-net/aspose.cells.rendering/sheetset#visible).|
| [draw_object_event_handler](/cells/fr/python-net/aspose.cells/paginatedsaveoptions/draw_object_event_handler) | Implémente cette interface pour obtenir DrawObject et Bound lors du rendu.|
| [page_saving_callback](/cells/fr/python-net/aspose.cells/paginatedsaveoptions/page_saving_callback) |Contrôler/indiquer la progression du processus d'enregistrement de la page.|



###  Voir également
* module [aspose.cells](..)
* classe [PaginatedSaveOptions](/cells/fr/python-net/aspose.cells/paginatedsaveoptions)
* classe [SaveOptions](/cells/fr/python-net/aspose.cells/saveoptions)
