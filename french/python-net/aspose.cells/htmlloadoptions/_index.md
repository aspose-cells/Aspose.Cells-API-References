---
title: HtmlLoadOptions classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 770
url: /fr/python-net/aspose.cells/htmlloadoptions/
is_root: false
---
##  HtmlLoadOptions classe
Représente les options lors de l'importation d'un fichier html.



**Héritage:** [HtmlLoadOptions](/cells/python-net/aspose.cells/htmlloadoptions) → 
[AbstractTextLoadOptions](/cells/python-net/aspose.cells/abstracttextloadoptions) → 
[LoadOptions](/cells/fr/python-net/aspose.cells/loadoptions)



Le type HtmlLoadOptions expose les membres suivants :

###  Constructeurs
| Constructeur| Description|
| :- | :- |
| [HtmlLoadOptions()](/cells/fr/python-net/aspose.cells/htmlloadoptions/__init__/#) | Crée une option de chargement du fichier.|
| [HtmlLoadOptions(load_format)](/cells/fr/python-net/aspose.cells/htmlloadoptions/__init__/#LoadFormat) | Crée une option de chargement du fichier.|


###  Propriétés
| Propriété| Description|
| :- | :- |
| [load_format](/cells/fr/python-net/aspose.cells/htmlloadoptions/load_format) | Obtient le format de chargement.|
| [password](/cells/fr/python-net/aspose.cells/htmlloadoptions/password) | Obtient et définit le mot de passe du classeur.|
| [parsing_formula_on_open](/cells/fr/python-net/aspose.cells/htmlloadoptions/parsing_formula_on_open) | Indique si l'analyse de la formule lors de la lecture du fichier.|
| [parsing_pivot_cached_records](/cells/fr/python-net/aspose.cells/htmlloadoptions/parsing_pivot_cached_records) | Indique si l'analyse du pivot a mis en cache les enregistrements lors du chargement du fichier.<br/> La valeur par défaut est faux.|
| [language_code](/cells/fr/python-net/aspose.cells/htmlloadoptions/language_code) | Obtient ou définit la langue de l'interface utilisateur de la version de Workbook basée sur CountryCode qui a enregistré le fichier.|
| [region](/cells/fr/python-net/aspose.cells/htmlloadoptions/region) | Obtient ou définit les paramètres régionaux du système en fonction de CountryCode au moment du chargement du fichier.|
| [default_style_settings](/cells/fr/python-net/aspose.cells/htmlloadoptions/default_style_settings) | Obtient les paramètres de style par défaut pour initialiser les styles du classeur|
| [standard_font](/cells/fr/python-net/aspose.cells/htmlloadoptions/standard_font) | Définit le nom de police standard par défaut|
| [standard_font_size](/cells/fr/python-net/aspose.cells/htmlloadoptions/standard_font_size) | Définit la taille de police standard par défaut.|
| [interrupt_monitor](/cells/fr/python-net/aspose.cells/htmlloadoptions/interrupt_monitor) | Obtient et définit le moniteur d'interruption.|
| [ignore_not_printed](/cells/fr/python-net/aspose.cells/htmlloadoptions/ignore_not_printed) | Ignorer les données qui ne sont pas imprimées en cas d'impression directe du fichier|
| [check_data_valid](/cells/fr/python-net/aspose.cells/htmlloadoptions/check_data_valid) | Vérifiez si les données sont valides dans le fichier modèle.|
| [check_excel_restriction](/cells/fr/python-net/aspose.cells/htmlloadoptions/check_excel_restriction) | Si vérifier la restriction du fichier Excel lorsque l'utilisateur modifie les objets liés aux cellules.<br/>Par exemple, Excel n'autorise pas la saisie d'une valeur de chaîne supérieure à 32 Ko.<br/>Lorsque vous saisissez une valeur supérieure à 32 Ko, par exemple Cell.PutValue(string), si cette propriété est vraie, vous obtiendrez une exception.<br/>Si cette propriété est fausse, nous accepterons votre valeur de chaîne d'entrée comme valeur de la cellule afin que plus tard<br/>vous pouvez générer la valeur de chaîne complète pour d'autres formats de fichier tels que CSV.<br/>Cependant, si vous avez défini un type de valeur non valide pour le format de fichier Excel,<br/> vous ne devez pas enregistrer le classeur au format de fichier Excel ultérieurement. Sinon, il peut y avoir une erreur inattendue pour le fichier Excel généré.|
| [keep_unparsed_data](/cells/fr/python-net/aspose.cells/htmlloadoptions/keep_unparsed_data) |Indique si les données non analysées sont conservées en mémoire pour le classeur lorsqu'il est chargé à partir du fichier de modèle. La valeur par défaut est true.|
| [load_filter](/cells/fr/python-net/aspose.cells/htmlloadoptions/load_filter) | Le filtre pour indiquer comment charger les données.|
| [light_cells_data_handler](/cells/fr/python-net/aspose.cells/htmlloadoptions/light_cells_data_handler) | Le gestionnaire de données pour le traitement des données des cellules lors de la lecture du fichier de modèle.|
| [memory_setting](/cells/fr/python-net/aspose.cells/htmlloadoptions/memory_setting) | Obtient ou définit les options d'utilisation de la mémoire.|
| [warning_callback](/cells/fr/python-net/aspose.cells/htmlloadoptions/warning_callback) | Obtient ou définit un rappel d'avertissement.|
| [auto_fitter_options](/cells/fr/python-net/aspose.cells/htmlloadoptions/auto_fitter_options) | Obtient et définit les options d'ajustement automatique|
| [auto_filter](/cells/fr/python-net/aspose.cells/htmlloadoptions/auto_filter) | Indique si le filtrage automatique des données lors du chargement des fichiers.|
| [font_configs](/cells/fr/python-net/aspose.cells/htmlloadoptions/font_configs) | Obtient et définit des configurations de police individuelles.<br/> Ne fonctionne que pour le [Workbook](/cells/fr/python-net/aspose.cells/workbook) qui utilise ce [LoadOptions](/cells/fr/python-net/aspose.cells/loadoptions) pour charger.|
| [encoding](/cells/fr/python-net/aspose.cells/htmlloadoptions/encoding) | Obtient et définit l'encodage par défaut. Ne s'applique qu'au fichier csv.|
| [load_style_strategy](/cells/fr/python-net/aspose.cells/htmlloadoptions/load_style_strategy) |Indique la stratégie pour appliquer le style aux valeurs analysées lors de la conversion d'une valeur de chaîne en nombre ou en date/heure.|
| [convert_numeric_data](/cells/fr/python-net/aspose.cells/htmlloadoptions/convert_numeric_data) | Obtient ou définit une valeur qui indique si la chaîne du fichier texte est convertie en données numériques.|
| [convert_date_time_data](/cells/fr/python-net/aspose.cells/htmlloadoptions/convert_date_time_data) | Obtient ou définit une valeur qui indique si la chaîne du fichier texte est convertie en données de date.|
| [keep_precision](/cells/fr/python-net/aspose.cells/htmlloadoptions/keep_precision) | Indique si une valeur de chaîne n'est pas analysée si la longueur est de 15.|
| [attached_files_directory](/cells/fr/python-net/aspose.cells/htmlloadoptions/attached_files_directory) | Le répertoire dans lequel les fichiers joints seront enregistrés.|
| [load_formulas](/cells/fr/python-net/aspose.cells/htmlloadoptions/load_formulas) | Indique si les formules sont importées si le fichier html d'origine contient des formules|
| [support_div_tag](/cells/fr/python-net/aspose.cells/htmlloadoptions/support_div_tag) | Indique si la prise en charge de la mise en page de<div> balise lorsque le fichier html contient<div> Mots clés. La valeur par défaut est faux.|
| [delete_redundant_spaces](/cells/fr/python-net/aspose.cells/htmlloadoptions/delete_redundant_spaces) | Indique si supprimer les espaces redondants lorsque le texte revient à la ligne à l'aide de<br> tag. La valeur par défaut est false.|
| [auto_fit_cols_and_rows](/cells/fr/python-net/aspose.cells/htmlloadoptions/auto_fit_cols_and_rows) | Indique si les colonnes et les lignes s'ajustent automatiquement. La valeur par défaut est faux.|
| [convert_formulas_data](/cells/fr/python-net/aspose.cells/htmlloadoptions/convert_formulas_data) | si vrai, convertit la chaîne en formule lorsque la valeur de la chaîne commence par le caractère '=', la valeur par défaut est fausse.|
| [stream_provider](/cells/fr/python-net/aspose.cells/htmlloadoptions/stream_provider) | Obtient ou définit le StreamProviderImportHtmlFile pour importer des objets.|
| [prog_id](/cells/fr/python-net/aspose.cells/htmlloadoptions/prog_id) | Obtient l'ID du programme de création du fichier.<br/> Uniquement pour les fichiers MHT.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [set_paper_size(type)](/cells/fr/python-net/aspose.cells/htmlloadoptions/set_paper_size/#PaperSizeType) | Définit le format de papier d'impression par défaut à partir des paramètres par défaut de l'imprimante.|



###  Voir également
* module [aspose.cells](..)
* classe [AbstractTextLoadOptions](/cells/fr/python-net/aspose.cells/abstracttextloadoptions)
* classe [HtmlLoadOptions](/cells/fr/python-net/aspose.cells/htmlloadoptions)
* classe [LoadOptions](/cells/fr/python-net/aspose.cells/loadoptions)
* classe [Workbook](/cells/fr/python-net/aspose.cells/workbook)
