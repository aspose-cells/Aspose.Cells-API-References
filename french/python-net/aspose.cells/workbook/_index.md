---
title: Workbook classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 1590
url: /fr/python-net/aspose.cells/workbook/
is_root: false
---
##  Workbook classe
Représente un objet racine pour créer une feuille de calcul Excel.



Le type Workbook expose les membres suivants :

###  Constructeurs
| Constructeur| Description|
| :- | :- |
| [Workbook()](/cells/fr/python-net/aspose.cells/workbook/__init__/#) | Initialise une nouvelle instance de la classe [Workbook](/cells/fr/python-net/aspose.cells/workbook).|
| [Workbook(file_format_type)](/cells/fr/python-net/aspose.cells/workbook/__init__/#FileFormatType) | Initialise une nouvelle instance de la classe [Workbook](/cells/fr/python-net/aspose.cells/workbook).|
| [Workbook(file)](/cells/fr/python-net/aspose.cells/workbook/__init__/#str) | Initialise une nouvelle instance de la classe [Workbook](/cells/fr/python-net/aspose.cells/workbook) et ouvre un fichier.|
| [Workbook(stream)](/cells/fr/python-net/aspose.cells/workbook/__init__/#io.RawIOBase) | Initialise une nouvelle instance de la classe [Workbook](/cells/fr/python-net/aspose.cells/workbook) et ouvre un flux.|
| [Workbook(file, load_options)](/cells/fr/python-net/aspose.cells/workbook/__init__/#str-LoadOptions) | Initialise une nouvelle instance de la classe [Workbook](/cells/fr/python-net/aspose.cells/workbook) et ouvre un fichier.|
| [Workbook(stream, load_options)](/cells/fr/python-net/aspose.cells/workbook/__init__/#io.RawIOBase-LoadOptions) | Initialise une nouvelle instance de la classe [Workbook](/cells/fr/python-net/aspose.cells/workbook) et du flux ouvert.|


###  Propriétés
| Propriété| Description|
| :- | :- |
| [settings](/cells/fr/python-net/aspose.cells/workbook/settings) | Représente les paramètres du classeur.|
| [worksheets](/cells/fr/python-net/aspose.cells/workbook/worksheets) | Obtient la collection [WorksheetCollection](/cells/fr/python-net/aspose.cells/worksheetcollection) dans la feuille de calcul.|
| [is_licensed](/cells/fr/python-net/aspose.cells/workbook/is_licensed) | Indique si la licence est définie.|
| [colors](/cells/fr/python-net/aspose.cells/workbook/colors) | Renvoie les couleurs dans la palette de la feuille de calcul.|
| [count_of_styles_in_pool](/cells/fr/python-net/aspose.cells/workbook/count_of_styles_in_pool) | Obtient le nombre de styles dans le pool de styles.|
| [default_style](/cells/fr/python-net/aspose.cells/workbook/default_style) | Obtient ou définit l'objet par défaut [Style](/cells/fr/python-net/aspose.cells/style) du classeur.|
| [is_digitally_signed](/cells/fr/python-net/aspose.cells/workbook/is_digitally_signed) | Indique si cette feuille de calcul est signée numériquement.|
| [is_workbook_protected_with_password](/cells/fr/python-net/aspose.cells/workbook/is_workbook_protected_with_password) | Indique si la structure ou la fenêtre est protégée par mot de passe.|
| [vba_project](/cells/fr/python-net/aspose.cells/workbook/vba_project) | Obtient le [Workbook.vba_project](/cells/fr/python-net/aspose.cells/workbook#vba_project) dans une feuille de calcul.|
| [has_macro](/cells/fr/python-net/aspose.cells/workbook/has_macro) | Indique si cette feuille de calcul contient macro/VBA.|
| [has_revisions](/cells/fr/python-net/aspose.cells/workbook/has_revisions) | Obtient si le classeur contient des modifications suivies|
| [file_name](/cells/fr/python-net/aspose.cells/workbook/file_name) |Obtient et définit le nom de fichier actuel.|
| [cells_data_table_factory](/cells/fr/python-net/aspose.cells/workbook/cells_data_table_factory) | Obtient la fabrique pour construire ICellsDataTable à partir d'objets personnalisés|
| [data_sorter](/cells/fr/python-net/aspose.cells/workbook/data_sorter) | Obtient un objet DataSorter pour trier les données.|
| [theme](/cells/fr/python-net/aspose.cells/workbook/theme) | Obtient le nom du thème.|
| [built_in_document_properties](/cells/fr/python-net/aspose.cells/workbook/built_in_document_properties) | Renvoie une collection [DocumentProperty](/cells/fr/python-net/aspose.cells.properties/documentproperty) qui représente toutes les propriétés de document intégrées de la feuille de calcul.|
| [custom_document_properties](/cells/fr/python-net/aspose.cells/workbook/custom_document_properties) | Renvoie une collection [DocumentProperty](/cells/fr/python-net/aspose.cells.properties/documentproperty) qui représente toutes les propriétés de document personnalisées de la feuille de calcul.|
| [file_format](/cells/fr/python-net/aspose.cells/workbook/file_format) | Obtient et définit le format de fichier.|
| [interrupt_monitor](/cells/fr/python-net/aspose.cells/workbook/interrupt_monitor) | Obtient et définit le moniteur d'interruption.|
| [content_type_properties](/cells/fr/python-net/aspose.cells/workbook/content_type_properties) | Obtient la liste des objets [ContentTypeProperty](/cells/fr/python-net/aspose.cells.properties/contenttypeproperty) dans le classeur.|
| [custom_xml_parts](/cells/fr/python-net/aspose.cells/workbook/custom_xml_parts) | Représente une partie de stockage de données XML personnalisée (données XML personnalisées dans un package).|
| [data_mashup](/cells/fr/python-net/aspose.cells/workbook/data_mashup) | Obtient des données de mashup.|
| [ribbon_xml](/cells/fr/python-net/aspose.cells/workbook/ribbon_xml) | Obtient et définit le fichier XML qui définit l'interface utilisateur du ruban.|
| [absolute_path](/cells/fr/python-net/aspose.cells/workbook/absolute_path) | Obtient et définit le chemin absolu du fichier.|
| [data_connections](/cells/fr/python-net/aspose.cells/workbook/data_connections) | Obtient la collection [ExternalConnection](/cells/fr/python-net/aspose.cells.externalconnections/externalconnection).|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [save(file_name, save_format)](/cells/fr/python-net/aspose.cells/workbook/save/#str-SaveFormat) | Enregistre le classeur sur le disque.|
| [save(file_name)](/cells/fr/python-net/aspose.cells/workbook/save/#str) | Enregistrez le classeur sur le disque.|
| [save(file_name, save_options)](/cells/fr/python-net/aspose.cells/workbook/save/#str-SaveOptions) | Enregistre le classeur sur le disque.|
| [save(stream, save_format)](/cells/fr/python-net/aspose.cells/workbook/save/#io.RawIOBase-SaveFormat) | Enregistre le classeur dans le flux.|
| [save(stream, save_options)](/cells/fr/python-net/aspose.cells/workbook/save/#io.RawIOBase-SaveOptions) | Enregistre le classeur dans le flux.|
| [replace(place_holder, new_value)](/cells/fr/python-net/aspose.cells/workbook/replace/#str-str) | Remplace la valeur d'une cellule par une nouvelle chaîne.|
| [replace(place_holder, new_value)](/cells/fr/python-net/aspose.cells/workbook/replace/#str-int) | Remplace la valeur d'une cellule par un nouvel entier.|
| [replace(place_holder, new_value)](/cells/fr/python-net/aspose.cells/workbook/replace/#str-float) |Remplace la valeur d'une cellule par un nouveau double.|
| [replace(place_holder, new_values, is_vertical)](/cells/fr/python-net/aspose.cells/workbook/replace/#str-list-bool) | Remplace la valeur d'une cellule par un nouveau tableau de chaînes.|
| [replace(place_holder, new_values, is_vertical)](/cells/fr/python-net/aspose.cells/workbook/replace/#str-list-bool) | Remplace les valeurs des cellules par un tableau d'entiers.|
| [replace(place_holder, new_values, is_vertical)](/cells/fr/python-net/aspose.cells/workbook/replace/#str-list-bool) | Remplace les valeurs des cellules par un double tableau.|
| [replace(bool_value, new_value)](/cells/fr/python-net/aspose.cells/workbook/replace/#bool-any) | Remplace les valeurs des cellules par de nouvelles données.|
| [replace(int_value, new_value)](/cells/fr/python-net/aspose.cells/workbook/replace/#int-any) | Remplace les valeurs des cellules par de nouvelles données.|
| [replace(place_holder, new_value, options)](/cells/fr/python-net/aspose.cells/workbook/replace/#str-str-ReplaceOptions) | Remplace la valeur d'une cellule par une nouvelle chaîne.|
| [copy(source, copy_options)](/cells/fr/python-net/aspose.cells/workbook/copy/#Workbook-CopyOptions) | Copie les données d'un objet Workbook source.|
| [copy(source)](/cells/fr/python-net/aspose.cells/workbook/copy/#Workbook) | Copie les données d'un objet Workbook source.|
| [calculate_formula()](/cells/fr/python-net/aspose.cells/workbook/calculate_formula/#) | Calcule le résultat de formules.|
| [calculate_formula(ignore_error)](/cells/fr/python-net/aspose.cells/workbook/calculate_formula/#bool) | Calcule le résultat de formules.|
| [calculate_formula(ignore_error, custom_function)](/cells/fr/python-net/aspose.cells/workbook/calculate_formula/#bool-ICustomFunction) | Calcule le résultat de formules.|
| [calculate_formula(options)](/cells/fr/python-net/aspose.cells/workbook/calculate_formula/#CalculationOptions) | Calculer des formules dans ce classeur.|
| [refresh_dynamic_array_formulas(calculate)](/cells/fr/python-net/aspose.cells/workbook/refresh_dynamic_array_formulas/#bool) | Actualise les formules de tableau dynamique (se répand dans une nouvelle plage de cellules voisines en fonction des données actuelles)<br/> Les autres formules du classeur ne seront pas calculées de manière récursive même si elles ont été utilisées par des formules matricielles dynamiques.|
| [refresh_dynamic_array_formulas(calculate, copts)](/cells/fr/python-net/aspose.cells/workbook/refresh_dynamic_array_formulas/#bool-CalculationOptions) | Actualise les formules de tableau dynamique (se répand dans une nouvelle plage de cellules voisines en fonction des données actuelles)|
| [import_xml(url, sheet_name, row, col)](/cells/fr/python-net/aspose.cells/workbook/import_xml/#str-str-int-int) | Importe/met à jour un fichier de données XML dans le classeur.|
| [import_xml(stream, sheet_name, row, col)](/cells/fr/python-net/aspose.cells/workbook/import_xml/#io.RawIOBase-str-int-int) | Importe/met à jour un fichier de données XML dans le classeur.|
| [export_xml(map_name, path)](/cells/fr/python-net/aspose.cells/workbook/export_xml/#str-str) | Exporter les données XML liées par le mappage XML spécifié.|
| [export_xml(map_name, stream)](/cells/fr/python-net/aspose.cells/workbook/export_xml/#str-io.RawIOBase) | Exporter des données XML.|
| [parse_formulas(ignore_error)](/cells/fr/python-net/aspose.cells/workbook/parse_formulas/#bool) | Analyse toutes les formules qui n'ont pas été analysées lorsqu'elles ont été chargées à partir d'un fichier de modèle ou définies dans une cellule.|
| [start_access_cache(opts)](/cells/fr/python-net/aspose.cells/workbook/start_access_cache/#AccessCacheOptions) |Démarre la session qui utilise les caches pour accéder aux données.|
| [close_access_cache(opts)](/cells/fr/python-net/aspose.cells/workbook/close_access_cache/#AccessCacheOptions) | Ferme la session qui utilise les caches pour accéder aux données.|
| [remove_unused_styles()](/cells/fr/python-net/aspose.cells/workbook/remove_unused_styles/#) | Supprimez tous les styles inutilisés.|
| [create_style()](/cells/fr/python-net/aspose.cells/workbook/create_style/#) | Crée un nouveau style.|
| [create_builtin_style(type)](/cells/fr/python-net/aspose.cells/workbook/create_builtin_style/#BuiltinStyleType) | Crée un style intégré par type donné.|
| [create_cells_color()](/cells/fr/python-net/aspose.cells/workbook/create_cells_color/#) | Crée un objet [CellsColor](/cells/fr/python-net/aspose.cells/cellscolor).|
| [combine(second_workbook)](/cells/fr/python-net/aspose.cells/workbook/combine/#Workbook) | Combine un autre objet Workbook.|
| [get_style_in_pool(index)](/cells/fr/python-net/aspose.cells/workbook/get_style_in_pool/#int) | Obtient le style dans le pool de styles.<br/>Tous les styles du classeur seront rassemblés dans un pool.<br/> Il n'y a qu'un simple index de référence dans les cellules.|
| [get_fonts()](/cells/fr/python-net/aspose.cells/workbook/get_fonts/#) | Obtient toutes les polices du pool de styles.|
| [get_named_style(name)](/cells/fr/python-net/aspose.cells/workbook/get_named_style/#str) | Obtient le style nommé dans le pool de styles.|
| [change_palette(color, index)](/cells/fr/python-net/aspose.cells/workbook/change_palette/#aspose.pydrawing.Color-int) | Modifie la palette de la feuille de calcul dans l'index spécifié.|
| [is_color_in_palette(color)](/cells/fr/python-net/aspose.cells/workbook/is_color_in_palette/#aspose.pydrawing.Color) | Vérifie si une couleur se trouve dans la palette de la feuille de calcul.|
| [get_matching_color(raw_color)](/cells/fr/python-net/aspose.cells/workbook/get_matching_color/#aspose.pydrawing.Color) | Trouvez la meilleure couleur correspondante dans la palette actuelle.|
| [set_encryption_options(encryption_type, key_length)](/cells/fr/python-net/aspose.cells/workbook/set_encryption_options/#EncryptionType-int) | Définissez les options de chiffrement.|
| [protect(protection_type, password)](/cells/fr/python-net/aspose.cells/workbook/protect/#ProtectionType-str) | Protège un classeur.|
| [protect_shared_workbook(password)](/cells/fr/python-net/aspose.cells/workbook/protect_shared_workbook/#str) | Protège un classeur partagé.|
| [unprotect(password)](/cells/fr/python-net/aspose.cells/workbook/unprotect/#str) | Déprotége un classeur.|
| [unprotect_shared_workbook(password)](/cells/fr/python-net/aspose.cells/workbook/unprotect_shared_workbook/#str) | Déprotége un classeur partagé.|
| [remove_macro()](/cells/fr/python-net/aspose.cells/workbook/remove_macro/#) | Supprime VBA/macro de cette feuille de calcul.|
| [remove_digital_signature()](/cells/fr/python-net/aspose.cells/workbook/remove_digital_signature/#) | Supprime la signature numérique de cette feuille de calcul.|
| [accept_all_revisions()](/cells/fr/python-net/aspose.cells/workbook/accept_all_revisions/#) | Accepte toutes les modifications suivies dans le classeur.|
| [remove_external_links()](/cells/fr/python-net/aspose.cells/workbook/remove_external_links/#) |Supprime tous les liens externes du classeur.|
| [get_theme_color(type)](/cells/fr/python-net/aspose.cells/workbook/get_theme_color/#ThemeColorType) | Obtient la couleur du thème.|
| [set_theme_color(type, color)](/cells/fr/python-net/aspose.cells/workbook/set_theme_color/#ThemeColorType-aspose.pydrawing.Color) | Définit la couleur du thème|
| [custom_theme(theme_name, colors)](/cells/fr/python-net/aspose.cells/workbook/custom_theme/#str-aspose.pydrawing.Color[]) | Customise le thème.|
| [copy_theme(source)](/cells/fr/python-net/aspose.cells/workbook/copy_theme/#Workbook) | Copie le thème d'un autre classeur.|
| [has_exernal_links()](/cells/fr/python-net/aspose.cells/workbook/has_exernal_links/#) | Indique si ce classeur contient des liens externes vers d'autres sources de données.|
| [update_linked_data_source(external_workbooks)](/cells/fr/python-net/aspose.cells/workbook/update_linked_data_source/#list) | Si ce classeur contient des liens externes vers d'autres sources de données,<br/> Aspose.Cells tentera de récupérer les dernières données.|
| [set_digital_signature(digital_signature_collection)](/cells/fr/python-net/aspose.cells/workbook/set_digital_signature/#aspose.cells.digitalsignatures.DigitalSignatureCollection) | Définit la signature numérique d'un fichier de feuille de calcul (Excel2007 et versions ultérieures).|
| [add_digital_signature(digital_signature_collection)](/cells/fr/python-net/aspose.cells/workbook/add_digital_signature/#aspose.cells.digitalsignatures.DigitalSignatureCollection) | Ajoute une signature numérique à un fichier de feuille de calcul OOXML (Excel2007 et versions ultérieures).|
| [get_digital_signature()](/cells/fr/python-net/aspose.cells/workbook/get_digital_signature/#) | Obtient la signature numérique du fichier.|
| [remove_personal_information()](/cells/fr/python-net/aspose.cells/workbook/remove_personal_information/#) | Supprime les informations personnelles.|



###  Remarques

La classe Workbook désigne une feuille de calcul Excel.
La fonctionnalité de base de la classe est d'ouvrir et d'enregistrer des fichiers Excel natifs.
La classe possède des fonctionnalités avancées telles que la copie de données à partir d'autres classeurs, la combinaison de deux classeurs et la protection de la feuille de calcul Excel.

###  Exemples

L'exemple suivant charge un Workbook à partir d'un fichier nommé designer.xls et rend les barres de défilement horizontale et verticale invisibles pour le Workbook. Il remplace ensuite deux valeurs de chaîne par une valeur entière et une valeur de chaîne respectivement dans la feuille de calcul et envoie enfin la mise à jour fichier au navigateur client.

```python
from aspose.cells import Workbook

# Open a designer file
designerFile = "designer.xls"
workbook = Workbook(designerFile)
# Set scroll bars
workbook.settings.is_h_scroll_bar_visible = False
workbook.settings.is_v_scroll_bar_visible = False
# Replace the placeholder string with new values
newInt = 100
workbook.replace("OldInt", newInt)
newString = "Hello!"
workbook.replace("OldString", newString)
workbook.save("result.xls")

```

###  Voir également
* module [aspose.cells](..)
* classe [CellsColor](/cells/fr/python-net/aspose.cells/cellscolor)
* classe [ContentTypeProperty](/cells/fr/python-net/aspose.cells.properties/contenttypeproperty)
* classe [DocumentProperty](/cells/fr/python-net/aspose.cells.properties/documentproperty)
* classe [ExternalConnection](/cells/fr/python-net/aspose.cells.externalconnections/externalconnection)
* classe [Style](/cells/fr/python-net/aspose.cells/style)
* classe [Workbook](/cells/fr/python-net/aspose.cells/workbook)
* classe [WorksheetCollection](/cells/fr/python-net/aspose.cells/worksheetcollection)
