---
title: HtmlSaveOptions classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 780
url: /fr/python-net/aspose.cells/htmlsaveoptions/
is_root: false
---
##  HtmlSaveOptions classe
Représente les options d'enregistrement du fichier html.



**Héritage:** [HtmlSaveOptions](/cells/python-net/aspose.cells/htmlsaveoptions) → 
[SaveOptions](/cells/fr/python-net/aspose.cells/saveoptions)



Le type HtmlSaveOptions expose les membres suivants :

###  Constructeurs
| Constructeur| Description|
| :- | :- |
| [HtmlSaveOptions()](/cells/fr/python-net/aspose.cells/htmlsaveoptions/__init__/#) | Crée des options pour enregistrer le fichier html.|
| [HtmlSaveOptions(format)](/cells/fr/python-net/aspose.cells/htmlsaveoptions/__init__/#SaveFormat) | Crée des options pour enregistrer le fichier htm.|


###  Propriétés
| Propriété| Description|
| :- | :- |
| [save_format](/cells/fr/python-net/aspose.cells/htmlsaveoptions/save_format) | Obtient le format du fichier de sauvegarde.|
| [clear_data](/cells/fr/python-net/aspose.cells/htmlsaveoptions/clear_data) | Videz le classeur après avoir enregistré le fichier.|
| [cached_file_folder](/cells/fr/python-net/aspose.cells/htmlsaveoptions/cached_file_folder) | Le dossier de fichiers mis en cache est utilisé pour stocker des données volumineuses.|
| [validate_merged_areas](/cells/fr/python-net/aspose.cells/htmlsaveoptions/validate_merged_areas) | Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier.|
| [merge_areas](/cells/fr/python-net/aspose.cells/htmlsaveoptions/merge_areas) | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier.|
| [create_directory](/cells/fr/python-net/aspose.cells/htmlsaveoptions/create_directory) | Si true et que le répertoire n'existe pas, le répertoire sera automatiquement créé avant d'enregistrer le fichier.|
| [sort_names](/cells/fr/python-net/aspose.cells/htmlsaveoptions/sort_names) | Indique s'il faut trier les noms définis avant d'enregistrer le fichier.|
| [sort_external_names](/cells/fr/python-net/aspose.cells/htmlsaveoptions/sort_external_names) | Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier.|
| [refresh_chart_cache](/cells/fr/python-net/aspose.cells/htmlsaveoptions/refresh_chart_cache) |Indique si l'actualisation des données du cache du graphique|
| [warning_callback](/cells/fr/python-net/aspose.cells/htmlsaveoptions/warning_callback) | Obtient ou définit un rappel d'avertissement.|
| [update_smart_art](/cells/fr/python-net/aspose.cells/htmlsaveoptions/update_smart_art) | Indique si la mise à jour du paramètre d'art intelligent.<br/> La valeur par défaut est faux.|
| [ignore_invisible_shapes](/cells/fr/python-net/aspose.cells/htmlsaveoptions/ignore_invisible_shapes) | Indiquez si vous exportez ces formes non visibles|
| [page_title](/cells/fr/python-net/aspose.cells/htmlsaveoptions/page_title) | Le titre de la page html.<br/> Uniquement pour enregistrer dans un flux html.|
| [attached_files_directory](/cells/fr/python-net/aspose.cells/htmlsaveoptions/attached_files_directory) |Le répertoire dans lequel les fichiers joints seront enregistrés.<br/> Uniquement pour enregistrer dans un flux html.|
| [attached_files_url_prefix](/cells/fr/python-net/aspose.cells/htmlsaveoptions/attached_files_url_prefix) | Spécifiez le préfixe d'URL des fichiers joints tels que l'image dans le fichier html.<br/> Uniquement pour enregistrer dans un flux html.|
| [default_font_name](/cells/fr/python-net/aspose.cells/htmlsaveoptions/default_font_name) | Spécifiez le nom de la police par défaut pour l'exportation html, la police par défaut sera utilisée lorsque la police de style n'existe pas,<br/>Si cette propriété est nulle, Aspose.Cells utilisera la police universelle qui a la même famille que la police d'origine,<br/> la valeur par défaut est nulle.|
| [worksheet_scalable](/cells/fr/python-net/aspose.cells/htmlsaveoptions/worksheet_scalable) |Indique si un zoom avant ou arrière sur le HTML via le niveau de zoom de la feuille de calcul lors de l'enregistrement du fichier au format HTML, la valeur par défaut est false.|
| [is_export_comments](/cells/fr/python-net/aspose.cells/htmlsaveoptions/is_export_comments) | Indique si l'exportation des commentaires lors de l'enregistrement du fichier au format html, la valeur par défaut est false.|
| [export_comments_type](/cells/fr/python-net/aspose.cells/htmlsaveoptions/export_comments_type) | Représente le type d'exportation de commentaires vers des fichiers html.|
| [disable_downlevel_revealed_comments](/cells/fr/python-net/aspose.cells/htmlsaveoptions/disable_downlevel_revealed_comments) | Indique si désactiver les commentaires conditionnels révélés par le niveau inférieur lors de l'exportation du fichier au format HTML, la valeur par défaut est false.|
| [is_exp_image_to_temp_dir](/cells/fr/python-net/aspose.cells/htmlsaveoptions/is_exp_image_to_temp_dir) | Indique si les fichiers image sont exportés vers le répertoire temporaire.<br/> Uniquement pour enregistrer dans un flux html.|
| [image_scalable](/cells/fr/python-net/aspose.cells/htmlsaveoptions/image_scalable) | Indique si l'unité évolutive est utilisée pour décrire la largeur de l'image<br/>lors de l'utilisation d'une unité évolutive pour décrire la largeur de la colonne.<br/> La valeur par défaut est true.|
| [width_scalable](/cells/fr/python-net/aspose.cells/htmlsaveoptions/width_scalable) | Indique si l'unité évolutive est utilisée pour décrire la largeur de la colonne lors de l'exportation du fichier au format HTML.<br/> La valeur par défaut est faux.|
| [export_single_tab](/cells/fr/python-net/aspose.cells/htmlsaveoptions/export_single_tab) | Indique s'il faut exporter l'onglet unique lorsque le fichier ne contient qu'une seule feuille de calcul.<br/> La valeur par défaut est faux.|
| [export_images_as_base64](/cells/fr/python-net/aspose.cells/htmlsaveoptions/export_images_as_base64) | Spécifie si les images sont enregistrées au format Base64 dans HTML, MHTML ou EPUB.|
| [export_active_worksheet_only](/cells/fr/python-net/aspose.cells/htmlsaveoptions/export_active_worksheet_only) | Indique si l'intégralité du classeur est exportée vers un fichier html.|
| [export_print_area_only](/cells/fr/python-net/aspose.cells/htmlsaveoptions/export_print_area_only) | Indique s'il s'agit d'exporter uniquement la zone d'impression vers un fichier html. La valeur par défaut est faux.|
| [export_area](/cells/fr/python-net/aspose.cells/htmlsaveoptions/export_area) | Obtient ou définit la CellArea d'exportation de la feuille de calcul active actuelle.<br/>Si vous définissez cet attribut, la zone d'impression de la feuille de calcul active actuelle sera omise.<br/> Seule la zone spécifiée sera exportée lors de l'enregistrement du fichier au format HTML.|
| [parse_html_tag_in_cell](/cells/fr/python-net/aspose.cells/htmlsaveoptions/parse_html_tag_in_cell) | Analyser la balise html dans la cellule, comme, comme valeur de cellule, ou comme balise html, la valeur par défaut est true|
| [html_cross_string_type](/cells/fr/python-net/aspose.cells/htmlsaveoptions/html_cross_string_type) | Indique si une chaîne intercellulaire sera affichée de la même manière que MS Excel lors de l'enregistrement d'un fichier Excel au format html.<br/>Par défaut, la valeur est Default, donc, pour les chaînes inter-cellules, il y a peu de différence entre les fichiers html créés par Aspose.Cells et MS Excel.<br/>Mais la performance pour créer de gros fichiers html, définir la valeur sur Cross serait plusieurs fois plus rapide que de la définir sur Default ou Fit2Cell.|
| [hidden_col_display_type](/cells/fr/python-net/aspose.cells/htmlsaveoptions/hidden_col_display_type) | Colonne masquée (la largeur de cette colonne est 0) dans Excel, avant de l'enregistrer au format html,<br/>si HtmlHiddenColDisplayType est "Supprimer", la colonne masquée ne sera pas sortie,<br/> si la valeur est "Hidden", la colonne serait sortie, mais était masquée, la valeur par défaut est "Hidden"|
| [hidden_row_display_type](/cells/fr/python-net/aspose.cells/htmlsaveoptions/hidden_row_display_type) | Ligne masquée (la hauteur de cette ligne est 0) dans Excel, avant de l'enregistrer au format html,<br/>si HtmlHiddenRowDisplayType est "Remove", la ligne masquée ne sera pas sortie,<br/> si la valeur est "Hidden", la ligne serait sortie, mais était masquée, la valeur par défaut est "Hidden"|
| [encoding](/cells/fr/python-net/aspose.cells/htmlsaveoptions/encoding) | S'il n'est pas défini, utilisez Encoding.UTF8 comme type d'encodage par défaut.|
| [export_object_listener](/cells/fr/python-net/aspose.cells/htmlsaveoptions/export_object_listener) | Obtient ou définit ExportObjectListener pour l'exportation d'objets.|
| [file_path_provider](/cells/fr/python-net/aspose.cells/htmlsaveoptions/file_path_provider) | Obtient ou définit le IFilePathProvider pour exporter la feuille de travail au format HTML séparément.|
| [stream_provider](/cells/fr/python-net/aspose.cells/htmlsaveoptions/stream_provider) | Obtient ou définit le IStreamProvider pour l'exportation d'objets.|
| [image_options](/cells/fr/python-net/aspose.cells/htmlsaveoptions/image_options) | Obtenir l'objet ImageOrPrintOptions avant l'exportation|
| [save_as_single_file](/cells/fr/python-net/aspose.cells/htmlsaveoptions/save_as_single_file) | Indique si enregistrer le HTML en tant que fichier unique.<br/> La valeur par défaut est faux.|
| [show_all_sheets](/cells/fr/python-net/aspose.cells/htmlsaveoptions/show_all_sheets) | Indique si toutes les feuilles sont affichées lors de l'enregistrement en un seul fichier html.|
| [export_page_headers](/cells/fr/python-net/aspose.cells/htmlsaveoptions/export_page_headers) | Indique si les en-têtes de page sont exportés.|
| [export_page_footers](/cells/fr/python-net/aspose.cells/htmlsaveoptions/export_page_footers) | Indique si les en-têtes de page sont exportés.|
| [export_hidden_worksheet](/cells/fr/python-net/aspose.cells/htmlsaveoptions/export_hidden_worksheet) |Indique si le contenu masqué de la feuille de calcul est exporté. La valeur par défaut est true.|
| [presentation_preference](/cells/fr/python-net/aspose.cells/htmlsaveoptions/presentation_preference) | Indique si le fichier html ou mht est la préférence de présentation.<br/>La valeur par défaut est faux.<br/> Si vous souhaitez obtenir une présentation plus belle, veuillez définir la valeur sur true.|
| [cell_css_prefix](/cells/fr/python-net/aspose.cells/htmlsaveoptions/cell_css_prefix) | Obtient et définit le préfixe du nom CSS, la valeur par défaut est "".|
| [table_css_id](/cells/fr/python-net/aspose.cells/htmlsaveoptions/table_css_id) |Obtient et définit le préfixe du nom de type css tel que tr, col, td et ainsi de suite, ils sont contenus dans l'élément table<br/> qui a l'attribut TableCssId spécifique. La valeur par défaut est "".|
| [is_full_path_link](/cells/fr/python-net/aspose.cells/htmlsaveoptions/is_full_path_link) | Indique si vous utilisez un lien de chemin complet dans sheet00x.htm,filelist.xml et tabstrip.htm.<br/> La valeur par défaut est faux.|
| [export_worksheet_css_separately](/cells/fr/python-net/aspose.cells/htmlsaveoptions/export_worksheet_css_separately) | Indique si vous exportez la feuille de calcul CSS séparément. La valeur par défaut est false.|
| [export_similar_border_style](/cells/fr/python-net/aspose.cells/htmlsaveoptions/export_similar_border_style) | Indique si le style de bordure similaire est exporté lorsque le style de bordure n'est pas pris en charge par les navigateurs.<br/>Si vous souhaitez importer le fichier html ou mht vers Excel, veuillez conserver la valeur par défaut.<br/> La valeur par défaut est faux.|
| [merge_empty_td_forcely](/cells/fr/python-net/aspose.cells/htmlsaveoptions/merge_empty_td_forcely) | Indique si la fusion forcée d'un élément TD vide lors de l'exportation du fichier au format HTML.<br/> La taille du fichier html sera considérablement réduite après avoir défini la valeur sur true. La valeur par défaut est faux.<br/> Si vous souhaitez importer le fichier html vers Excel ou exporter des lignes de grille parfaites lors de l'enregistrement du fichier au format html,<br/> veuillez conserver la valeur par défaut.|
| [export_cell_coordinate](/cells/fr/python-net/aspose.cells/htmlsaveoptions/export_cell_coordinate) | Indique si l'exportation des coordonnées Excel des cellules non vides lors de l'enregistrement du fichier au format HTML. La valeur par défaut est faux.<br/> Si vous souhaitez importer la sortie html vers Excel, veuillez conserver la valeur par défaut.|
| [export_extra_headings](/cells/fr/python-net/aspose.cells/htmlsaveoptions/export_extra_headings) | Indique s'il faut exporter des en-têtes supplémentaires lorsque la longueur du texte dépasse la colonne d'affichage maximale.<br/> La valeur par défaut est faux. Si vous souhaitez importer le fichier html vers Excel, veuillez conserver la valeur par défaut.|
| [export_headings](/cells/fr/python-net/aspose.cells/htmlsaveoptions/export_headings) | Indique si les en-têtes de ligne et de colonne de la feuille sont exportés lors de l'enregistrement dans des fichiers HTML.|
| [export_row_column_headings](/cells/fr/python-net/aspose.cells/htmlsaveoptions/export_row_column_headings) | Indique si les en-têtes de ligne et de colonne de la feuille sont exportés lors de l'enregistrement dans des fichiers HTML.|
| [export_formula](/cells/fr/python-net/aspose.cells/htmlsaveoptions/export_formula) | Indique si la formule est exportée lors de l'enregistrement du fichier au format HTML. La valeur par défaut est true.<br/> Si vous souhaitez importer la sortie html vers Excel, veuillez conserver la valeur par défaut.|
| [add_tooltip_text](/cells/fr/python-net/aspose.cells/htmlsaveoptions/add_tooltip_text) |Indique s'il faut ajouter du texte d'info-bulle lorsque les données ne peuvent pas être entièrement affichées.<br/> La valeur par défaut est faux.|
| [export_grid_lines](/cells/fr/python-net/aspose.cells/htmlsaveoptions/export_grid_lines) | Indique si le quadrillage est exporté. La valeur par défaut est false.|
| [export_bogus_row_data](/cells/fr/python-net/aspose.cells/htmlsaveoptions/export_bogus_row_data) | Indique si l'exportation de fausses données de la ligne inférieure est en cours. La valeur par défaut est true.Si vous souhaitez importer le fichier html ou mht<br/> pour exceller, veuillez conserver la valeur par défaut.|
| [exclude_unused_styles](/cells/fr/python-net/aspose.cells/htmlsaveoptions/exclude_unused_styles) | Indique si exclut les styles inutilisés.<br/>Pour les fichiers html générés, l'exclusion des styles inutilisés peut réduire la taille du fichier<br/>sans affecter les effets visuels. La valeur par défaut de cette propriété est donc true.<br/>Si l'utilisateur doit conserver tous les styles dans le classeur pour le code HTML généré (comme le scénario que l'utilisateur<br/> doit restaurer le classeur à partir du code HTML généré ultérieurement), veuillez définir cette propriété sur false.|
| [export_document_properties](/cells/fr/python-net/aspose.cells/htmlsaveoptions/export_document_properties) | Indique si les propriétés du document sont exportées.La valeur par défaut est true.Si vous souhaitez importer<br/> le fichier html ou mht vers excel, veuillez conserver la valeur par défaut.|
| [export_worksheet_properties](/cells/fr/python-net/aspose.cells/htmlsaveoptions/export_worksheet_properties) | Indique si les propriétés de la feuille de calcul sont exportées.La valeur par défaut est true.Si vous souhaitez importer<br/> le fichier html ou mht vers excel, veuillez conserver la valeur par défaut.|
| [export_workbook_properties](/cells/fr/python-net/aspose.cells/htmlsaveoptions/export_workbook_properties) | Indique si les propriétés du classeur sont exportées. La valeur par défaut est true. Si vous souhaitez importer<br/> le fichier html ou mht vers excel, veuillez conserver la valeur par défaut.|
| [export_frame_scripts_and_properties](/cells/fr/python-net/aspose.cells/htmlsaveoptions/export_frame_scripts_and_properties) | Indique si les scripts de cadre et les propriétés du document sont exportés. La valeur par défaut est true.Si vous souhaitez importer le fichier html ou mht<br/> pour exceller, veuillez conserver la valeur par défaut.|
| [export_data_options](/cells/fr/python-net/aspose.cells/htmlsaveoptions/export_data_options) | Indique la règle d'exportation des données du fichier html. La valeur par défaut est Tout.|
| [link_target_type](/cells/fr/python-net/aspose.cells/htmlsaveoptions/link_target_type) | Indiquer le type d'attribut cible dans<a> lien, la valeur par défaut est HtmlLinkTargetType.Parent.|



###  Voir également
* module [aspose.cells](..)
* classe [HtmlSaveOptions](/cells/fr/python-net/aspose.cells/htmlsaveoptions)
* classe [SaveOptions](/cells/fr/python-net/aspose.cells/saveoptions)
