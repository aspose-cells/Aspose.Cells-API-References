---
title: PdfSaveOptions classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 1180
url: /fr/python-net/aspose.cells/pdfsaveoptions/
is_root: false
---
##  PdfSaveOptions classe
Représente les options d'enregistrement des fichiers pdf.



**Héritage:** [PdfSaveOptions](/cells/python-net/aspose.cells/pdfsaveoptions) → 
[PaginatedSaveOptions](/cells/python-net/aspose.cells/paginatedsaveoptions) → 
[SaveOptions](/cells/fr/python-net/aspose.cells/saveoptions)



Le type PdfSaveOptions expose les membres suivants :

###  Constructeurs
| Constructeur| Description|
| :- | :- |
| [PdfSaveOptions()](/cells/fr/python-net/aspose.cells/pdfsaveoptions/__init__/#) | Crée les options d'enregistrement des fichiers pdf.|


###  Propriétés
| Propriété| Description|
| :- | :- |
| [save_format](/cells/fr/python-net/aspose.cells/pdfsaveoptions/save_format) | Obtient le format du fichier de sauvegarde.|
| [clear_data](/cells/fr/python-net/aspose.cells/pdfsaveoptions/clear_data) | Videz le classeur après avoir enregistré le fichier.|
| [cached_file_folder](/cells/fr/python-net/aspose.cells/pdfsaveoptions/cached_file_folder) | Le dossier de fichiers mis en cache est utilisé pour stocker des données volumineuses.|
| [validate_merged_areas](/cells/fr/python-net/aspose.cells/pdfsaveoptions/validate_merged_areas) | Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier.|
| [merge_areas](/cells/fr/python-net/aspose.cells/pdfsaveoptions/merge_areas) | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier.|
| [create_directory](/cells/fr/python-net/aspose.cells/pdfsaveoptions/create_directory) | Si true et que le répertoire n'existe pas, le répertoire sera automatiquement créé avant d'enregistrer le fichier.|
| [sort_names](/cells/fr/python-net/aspose.cells/pdfsaveoptions/sort_names) | Indique s'il faut trier les noms définis avant d'enregistrer le fichier.|
| [sort_external_names](/cells/fr/python-net/aspose.cells/pdfsaveoptions/sort_external_names) |Indique s'il faut trier les noms définis en externe avant d'enregistrer le fichier.|
| [refresh_chart_cache](/cells/fr/python-net/aspose.cells/pdfsaveoptions/refresh_chart_cache) | Indique si l'actualisation des données du cache du graphique|
| [warning_callback](/cells/fr/python-net/aspose.cells/pdfsaveoptions/warning_callback) | Obtient ou définit des rappels d'avertissement.|
| [update_smart_art](/cells/fr/python-net/aspose.cells/pdfsaveoptions/update_smart_art) | Indique si la mise à jour du paramètre d'art intelligent.<br/> La valeur par défaut est faux.|
| [default_font](/cells/fr/python-net/aspose.cells/pdfsaveoptions/default_font) | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule,<br/>Ils peuvent apparaître sous forme de bloc dans pdf, image.<br/>Définissez la police par défaut telle que MingLiu ou MS Gothic pour afficher ces caractères.<br/> Si cette propriété n'est pas définie, Aspose.Cells utilisera la police par défaut du système pour afficher ces caractères Unicode.|
| [check_workbook_default_font](/cells/fr/python-net/aspose.cells/pdfsaveoptions/check_workbook_default_font) | Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule,<br/>Ils peuvent apparaître sous forme de bloc dans pdf, image.<br/> Définissez ceci sur true pour essayer d'utiliser la police par défaut du classeur pour afficher ces caractères en premier.|
| [check_font_compatibility](/cells/fr/python-net/aspose.cells/pdfsaveoptions/check_font_compatibility) |Indique s'il faut vérifier la compatibilité des polices pour chaque caractère du texte.|
| [is_font_substitution_char_granularity](/cells/fr/python-net/aspose.cells/pdfsaveoptions/is_font_substitution_char_granularity) | Indique s'il faut uniquement remplacer la police de caractère lorsque la police de la cellule n'est pas compatible avec celle-ci.|
| [one_page_per_sheet](/cells/fr/python-net/aspose.cells/pdfsaveoptions/one_page_per_sheet) | Si OnePagePerSheet est true , tout le contenu d'une feuille sortira sur une seule page dans le résultat.<br/> Le format de papier de pagesetup sera invalide, et les autres paramètres de pagesetup<br/> prendra toujours effet.|
| [all_columns_in_one_page_per_sheet](/cells/fr/python-net/aspose.cells/pdfsaveoptions/all_columns_in_one_page_per_sheet) | Si AllColumnsInOnePagePerSheet est true , tout le contenu de la colonne d'une feuille sortira sur une seule page dans le résultat.<br/> La largeur de la taille du papier de pagesetup sera ignorée, et les autres paramètres de pagesetup<br/> prendra toujours effet.|
| [ignore_error](/cells/fr/python-net/aspose.cells/pdfsaveoptions/ignore_error) | Indique si vous devez masquer l'erreur lors du rendu.<br/> L'erreur peut être une erreur de forme, d'image, de rendu graphique, etc.|
| [output_blank_page_when_nothing_to_print](/cells/fr/python-net/aspose.cells/pdfsaveoptions/output_blank_page_when_nothing_to_print) | Indique s'il faut imprimer une page vierge lorsqu'il n'y a rien à imprimer.|
| [page_index](/cells/fr/python-net/aspose.cells/pdfsaveoptions/page_index) | Obtient ou définit l'index de base 0 de la première page à enregistrer.|
| [page_count](/cells/fr/python-net/aspose.cells/pdfsaveoptions/page_count) | Obtient ou définit le nombre de pages à enregistrer.|
| [printing_page_type](/cells/fr/python-net/aspose.cells/pdfsaveoptions/printing_page_type) | Indique quelles pages ne seront pas imprimées.|
| [gridline_type](/cells/fr/python-net/aspose.cells/pdfsaveoptions/gridline_type) | Obtient ou définit le type de quadrillage.|
| [text_cross_type](/cells/fr/python-net/aspose.cells/pdfsaveoptions/text_cross_type) | Obtient ou définit l'affichage du type de texte lorsque la largeur du texte est supérieure à la largeur de la cellule.|
| [default_edit_language](/cells/fr/python-net/aspose.cells/pdfsaveoptions/default_edit_language) | Obtient ou définit la langue d'édition par défaut.|
| [sheet_set](/cells/fr/python-net/aspose.cells/pdfsaveoptions/sheet_set) |Obtient ou définit les feuilles à afficher. La valeur par défaut est toutes les feuilles visibles dans le classeur : [SheetSet.visible](/cells/fr/python-net/aspose.cells.rendering/sheetset#visible).|
| [draw_object_event_handler](/cells/fr/python-net/aspose.cells/pdfsaveoptions/draw_object_event_handler) | Implémente cette interface pour obtenir DrawObject et Bound lors du rendu.|
| [page_saving_callback](/cells/fr/python-net/aspose.cells/pdfsaveoptions/page_saving_callback) | Contrôler/indiquer la progression du processus d'enregistrement de la page.|
| [embed_standard_windows_fonts](/cells/fr/python-net/aspose.cells/pdfsaveoptions/embed_standard_windows_fonts) | True pour incorporer des polices True Type.<br/>Affecte uniquement les caractères ASCII 32-127.<br/>Les polices pour les codes de caractères supérieurs à 127 sont toujours intégrées.<br/>Les polices sont toujours intégrées pour la norme PDF/A-1a, PDF/A-1b.<br/> La valeur par défaut est true.|
| [bookmark](/cells/fr/python-net/aspose.cells/pdfsaveoptions/bookmark) |Obtient et définit l'objet [PdfBookmarkEntry](/cells/fr/python-net/aspose.cells.rendering/pdfbookmarkentry).|
| [compliance](/cells/fr/python-net/aspose.cells/pdfsaveoptions/compliance) | Le classeur se convertit en pdf selon PdfCompliance dans cette propriété.|
| [security_options](/cells/fr/python-net/aspose.cells/pdfsaveoptions/security_options) | Définissez ces options, lorsque la sécurité est nécessaire dans le résultat xls2pdf.|
| [image_type](/cells/fr/python-net/aspose.cells/pdfsaveoptions/image_type) | Représente le type d'image lors de la conversion du graphique et de la forme.|
| [calculate_formula](/cells/fr/python-net/aspose.cells/pdfsaveoptions/calculate_formula) | Indique s'il faut calculer les formules avant d'enregistrer le fichier pdf.|
| [pdf_compression](/cells/fr/python-net/aspose.cells/pdfsaveoptions/pdf_compression) | Indiquez l'algorithme de compression|
| [created_time](/cells/fr/python-net/aspose.cells/pdfsaveoptions/created_time) | Obtient et définit l'heure de génération du document pdf.|
| [producer](/cells/fr/python-net/aspose.cells/pdfsaveoptions/producer) | Obtient et définit le producteur du document pdf généré.|
| [optimization_type](/cells/fr/python-net/aspose.cells/pdfsaveoptions/optimization_type) | Obtient et définit le type d'optimisation pdf.|
| [custom_properties_export](/cells/fr/python-net/aspose.cells/pdfsaveoptions/custom_properties_export) | Obtient ou définit une valeur déterminant la façon dont [CustomDocumentPropertyCollection](/cells/fr/python-net/aspose.cells.properties/customdocumentpropertycollection) sont exportés vers le fichier PDF. La valeur par défaut est Aucune.|
| [export_document_structure](/cells/fr/python-net/aspose.cells/pdfsaveoptions/export_document_structure) | Indique s'il faut exporter la structure du document.|
| [emf_render_setting](/cells/fr/python-net/aspose.cells/pdfsaveoptions/emf_render_setting) | Paramètre pour le rendu du métafichier Emf.|
| [display_doc_title](/cells/fr/python-net/aspose.cells/pdfsaveoptions/display_doc_title) | Indique si la barre de titre de la fenêtre doit afficher le titre du document.|
| [font_encoding](/cells/fr/python-net/aspose.cells/pdfsaveoptions/font_encoding) | Obtient ou définit l'encodage de police intégré dans le pdf.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [set_image_resample(desired_ppi, jpeg_quality)](/cells/fr/python-net/aspose.cells/pdfsaveoptions/set_image_resample/#int-int) | Définit le PPI souhaité (pixels par pouce) des images de rééchantillonnage et la qualité jpeg.<br/> Toutes les images seront converties en JPEG avec le paramètre de qualité spécifié,<br/>et les images supérieures au PPI spécifié (pixels par pouce) seront rééchantillonnées.|



###  Voir également
* module [aspose.cells](..)
* classe [CustomDocumentPropertyCollection](/cells/fr/python-net/aspose.cells.properties/customdocumentpropertycollection)
* classe [PaginatedSaveOptions](/cells/fr/python-net/aspose.cells/paginatedsaveoptions)
* classe [PdfBookmarkEntry](/cells/fr/python-net/aspose.cells.rendering/pdfbookmarkentry)
* classe [PdfSaveOptions](/cells/fr/python-net/aspose.cells/pdfsaveoptions)
* classe [SaveOptions](/cells/fr/python-net/aspose.cells/saveoptions)
