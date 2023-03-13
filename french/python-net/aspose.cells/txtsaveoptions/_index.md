---
title: TxtSaveOptions classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 1520
url: /fr/python-net/aspose.cells/txtsaveoptions/
is_root: false
---
##  TxtSaveOptions classe
Représente les options d'enregistrement pour csv/délimité par des tabulations/autre format de texte.



**Héritage:** [TxtSaveOptions](/cells/python-net/aspose.cells/txtsaveoptions) → 
[SaveOptions](/cells/fr/python-net/aspose.cells/saveoptions)



Le type TxtSaveOptions expose les membres suivants :

###  Constructeurs
| Constructeur| Description|
| :- | :- |
| [TxtSaveOptions()](/cells/fr/python-net/aspose.cells/txtsaveoptions/__init__/#) | Crée des options d'enregistrement de fichier texte.|
| [TxtSaveOptions(format)](/cells/fr/python-net/aspose.cells/txtsaveoptions/__init__/#SaveFormat) | Crée des options d'enregistrement de fichier texte.|


###  Propriétés
| Propriété| Description|
| :- | :- |
| [save_format](/cells/fr/python-net/aspose.cells/txtsaveoptions/save_format) | Obtient le format du fichier de sauvegarde.|
| [clear_data](/cells/fr/python-net/aspose.cells/txtsaveoptions/clear_data) | Videz le classeur après avoir enregistré le fichier.|
| [cached_file_folder](/cells/fr/python-net/aspose.cells/txtsaveoptions/cached_file_folder) | Le dossier de fichiers mis en cache est utilisé pour stocker des données volumineuses.|
| [validate_merged_areas](/cells/fr/python-net/aspose.cells/txtsaveoptions/validate_merged_areas) | Indique s'il faut valider les cellules fusionnées avant d'enregistrer le fichier.|
| [merge_areas](/cells/fr/python-net/aspose.cells/txtsaveoptions/merge_areas) | Indique s'il faut fusionner les zones de mise en forme conditionnelle et de validation avant d'enregistrer le fichier.|
| [create_directory](/cells/fr/python-net/aspose.cells/txtsaveoptions/create_directory) | Si true et que le répertoire n'existe pas, le répertoire sera automatiquement créé avant d'enregistrer le fichier.|
| [sort_names](/cells/fr/python-net/aspose.cells/txtsaveoptions/sort_names) | Indique s'il faut trier les noms définis avant d'enregistrer le fichier.|
| [sort_external_names](/cells/fr/python-net/aspose.cells/txtsaveoptions/sort_external_names) |Indique s'il faut trier les noms définis externes avant d'enregistrer le fichier.|
| [refresh_chart_cache](/cells/fr/python-net/aspose.cells/txtsaveoptions/refresh_chart_cache) | Indique si l'actualisation des données du cache du graphique|
| [warning_callback](/cells/fr/python-net/aspose.cells/txtsaveoptions/warning_callback) | Obtient ou définit un rappel d'avertissement.|
| [update_smart_art](/cells/fr/python-net/aspose.cells/txtsaveoptions/update_smart_art) | Indique si la mise à jour du paramètre d'art intelligent.<br/> La valeur par défaut est faux.|
| [separator](/cells/fr/python-net/aspose.cells/txtsaveoptions/separator) | Obtient et définit char Délimiteur de fichier texte.|
| [separator_string](/cells/fr/python-net/aspose.cells/txtsaveoptions/separator_string) | Obtient et définit une valeur de chaîne comme séparateur.|
| [encoding](/cells/fr/python-net/aspose.cells/txtsaveoptions/encoding) | Obtient et définit l'encodage par défaut.|
| [always_quoted](/cells/fr/python-net/aspose.cells/txtsaveoptions/always_quoted) | Indique s'il faut toujours ajouter '"' pour chaque champ.<br/>Si true, toutes les valeurs seront entre guillemets ;<br/>Si false, les valeurs ne seront entre guillemets que si nécessaire (par exemple,<br/>lorsque les valeurs contiennent des caractères spéciaux tels que '"' , '\n' ou un caractère de séparation).<br/> La valeur par défaut est false.|
| [quote_type](/cells/fr/python-net/aspose.cells/txtsaveoptions/quote_type) | Obtient ou définit comment citer des valeurs dans le fichier texte exporté.|
| [format_strategy](/cells/fr/python-net/aspose.cells/txtsaveoptions/format_strategy) | Obtient et définit la stratégie de format lors de l'exportation de la valeur de la cellule sous forme de chaîne.|
| [light_cells_data_provider](/cells/fr/python-net/aspose.cells/txtsaveoptions/light_cells_data_provider) | Le fournisseur de données pour fournir des données de cellules pour enregistrer le classeur en mode léger.|
| [trim_leading_blank_row_and_column](/cells/fr/python-net/aspose.cells/txtsaveoptions/trim_leading_blank_row_and_column) | Indique si les premières lignes et colonnes vides doivent être coupées comme ce que fait MS Excel.<br/> La valeur par défaut est true.|
| [trim_tailing_blank_cells](/cells/fr/python-net/aspose.cells/txtsaveoptions/trim_tailing_blank_cells) | Indique si les cellules vides de fin d'une ligne doivent être supprimées. La valeur par défaut est false.|
| [keep_separators_for_blank_row](/cells/fr/python-net/aspose.cells/txtsaveoptions/keep_separators_for_blank_row) | Indique si des séparateurs doivent être sortis pour une ligne vide.<br/> La valeur par défaut est false donc par défaut le contenu de la ligne vide sera vide.|
| [export_area](/cells/fr/python-net/aspose.cells/txtsaveoptions/export_area) | Plage de cellules à exporter.|
| [export_quote_prefix](/cells/fr/python-net/aspose.cells/txtsaveoptions/export_quote_prefix) | Indique si le guillemet simple doit être exporté dans le cadre de la valeur d'une cellule<br/> quand [Style.quote_prefix](/cells/fr/python-net/aspose.cells/style#quote_prefix) est vrai pour cela. La valeur par défaut est false.|
| [export_all_sheets](/cells/fr/python-net/aspose.cells/txtsaveoptions/export_all_sheets) |Indique si toutes les feuilles sont exportées vers le fichier texte.<br/> S'il est faux, exportez uniquement la feuille active, tout comme MS Excel.|



###  Voir également
* module [aspose.cells](..)
* classe [SaveOptions](/cells/fr/python-net/aspose.cells/saveoptions)
* classe [TxtSaveOptions](/cells/fr/python-net/aspose.cells/txtsaveoptions)
