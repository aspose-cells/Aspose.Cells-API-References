---
title: TxtLoadOptions classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 1510
url: /fr/python-net/aspose.cells/txtloadoptions/
is_root: false
---
##  TxtLoadOptions classe
Représente les options de chargement du fichier texte.



**Héritage:** [TxtLoadOptions](/cells/python-net/aspose.cells/txtloadoptions) → 
[AbstractTextLoadOptions](/cells/python-net/aspose.cells/abstracttextloadoptions) → 
[LoadOptions](/cells/fr/python-net/aspose.cells/loadoptions)



Le type TxtLoadOptions expose les membres suivants :

###  Constructeurs
| Constructeur| Description|
| :- | :- |
| [TxtLoadOptions()](/cells/fr/python-net/aspose.cells/txtloadoptions/__init__/#) | Crée les options de chargement du fichier texte.|
| [TxtLoadOptions(load_format)](/cells/fr/python-net/aspose.cells/txtloadoptions/__init__/#LoadFormat) | Crée les options de chargement du fichier texte.|


###  Propriétés
| Propriété| Description|
| :- | :- |
| [load_format](/cells/fr/python-net/aspose.cells/txtloadoptions/load_format) | Obtient le format de chargement.|
| [password](/cells/fr/python-net/aspose.cells/txtloadoptions/password) | Obtient et définit le mot de passe du classeur.|
| [parsing_formula_on_open](/cells/fr/python-net/aspose.cells/txtloadoptions/parsing_formula_on_open) | Indique si l'analyse de la formule lors de la lecture du fichier.|
| [parsing_pivot_cached_records](/cells/fr/python-net/aspose.cells/txtloadoptions/parsing_pivot_cached_records) | Indique si l'analyse du pivot a mis en cache les enregistrements lors du chargement du fichier.<br/> La valeur par défaut est faux.|
| [language_code](/cells/fr/python-net/aspose.cells/txtloadoptions/language_code) | Obtient ou définit la langue de l'interface utilisateur de la version de Workbook basée sur CountryCode qui a enregistré le fichier.|
| [region](/cells/fr/python-net/aspose.cells/txtloadoptions/region) | Obtient ou définit les paramètres régionaux du système en fonction de CountryCode au moment du chargement du fichier.|
| [default_style_settings](/cells/fr/python-net/aspose.cells/txtloadoptions/default_style_settings) | Obtient les paramètres de style par défaut pour initialiser les styles du classeur|
| [standard_font](/cells/fr/python-net/aspose.cells/txtloadoptions/standard_font) | Définit le nom de police standard par défaut|
| [standard_font_size](/cells/fr/python-net/aspose.cells/txtloadoptions/standard_font_size) | Définit la taille de police standard par défaut.|
| [interrupt_monitor](/cells/fr/python-net/aspose.cells/txtloadoptions/interrupt_monitor) | Obtient et définit le moniteur d'interruption.|
| [ignore_not_printed](/cells/fr/python-net/aspose.cells/txtloadoptions/ignore_not_printed) | Ignorer les données qui ne sont pas imprimées en cas d'impression directe du fichier|
| [check_data_valid](/cells/fr/python-net/aspose.cells/txtloadoptions/check_data_valid) | Vérifiez si les données sont valides dans le fichier modèle.|
| [check_excel_restriction](/cells/fr/python-net/aspose.cells/txtloadoptions/check_excel_restriction) | Si vérifier la restriction du fichier Excel lorsque l'utilisateur modifie les objets liés aux cellules.<br/>Par exemple, Excel n'autorise pas la saisie d'une valeur de chaîne supérieure à 32 Ko.<br/>Lorsque vous saisissez une valeur supérieure à 32 Ko, par exemple Cell.PutValue(string), si cette propriété est vraie, vous obtiendrez une exception.<br/>Si cette propriété est fausse, nous accepterons votre valeur de chaîne d'entrée comme valeur de la cellule afin que plus tard<br/>vous pouvez générer la valeur de chaîne complète pour d'autres formats de fichier tels que CSV.<br/>Cependant, si vous avez défini un type de valeur non valide pour le format de fichier Excel,<br/> vous ne devez pas enregistrer le classeur au format de fichier Excel ultérieurement. Sinon, il peut y avoir une erreur inattendue pour le fichier Excel généré.|
| [keep_unparsed_data](/cells/fr/python-net/aspose.cells/txtloadoptions/keep_unparsed_data) |Indique si les données non analysées sont conservées en mémoire pour le classeur lorsqu'il est chargé à partir du fichier de modèle. La valeur par défaut est true.|
| [load_filter](/cells/fr/python-net/aspose.cells/txtloadoptions/load_filter) | Le filtre pour indiquer comment charger les données.|
| [light_cells_data_handler](/cells/fr/python-net/aspose.cells/txtloadoptions/light_cells_data_handler) | Le gestionnaire de données pour le traitement des données des cellules lors de la lecture du fichier de modèle.|
| [memory_setting](/cells/fr/python-net/aspose.cells/txtloadoptions/memory_setting) | Obtient ou définit les options d'utilisation de la mémoire.|
| [warning_callback](/cells/fr/python-net/aspose.cells/txtloadoptions/warning_callback) | Obtient ou définit un rappel d'avertissement.|
| [auto_fitter_options](/cells/fr/python-net/aspose.cells/txtloadoptions/auto_fitter_options) | Obtient et définit les options d'ajustement automatique|
| [auto_filter](/cells/fr/python-net/aspose.cells/txtloadoptions/auto_filter) | Indique si le filtrage automatique des données lors du chargement des fichiers.|
| [font_configs](/cells/fr/python-net/aspose.cells/txtloadoptions/font_configs) | Obtient et définit des configurations de police individuelles.<br/> Ne fonctionne que pour le [Workbook](/cells/fr/python-net/aspose.cells/workbook) qui utilise ce [LoadOptions](/cells/fr/python-net/aspose.cells/loadoptions) pour charger.|
| [encoding](/cells/fr/python-net/aspose.cells/txtloadoptions/encoding) | Obtient et définit l'encodage par défaut. Ne s'applique qu'au fichier csv.|
| [load_style_strategy](/cells/fr/python-net/aspose.cells/txtloadoptions/load_style_strategy) |Indique la stratégie pour appliquer le style aux valeurs analysées lors de la conversion d'une valeur de chaîne en nombre ou en date/heure.|
| [convert_numeric_data](/cells/fr/python-net/aspose.cells/txtloadoptions/convert_numeric_data) | Obtient ou définit une valeur qui indique si la chaîne du fichier texte est convertie en données numériques.|
| [convert_date_time_data](/cells/fr/python-net/aspose.cells/txtloadoptions/convert_date_time_data) | Obtient ou définit une valeur qui indique si la chaîne du fichier texte est convertie en données de date.|
| [keep_precision](/cells/fr/python-net/aspose.cells/txtloadoptions/keep_precision) | Indique si une valeur de chaîne n'est pas analysée si la longueur est de 15.|
| [separator](/cells/fr/python-net/aspose.cells/txtloadoptions/separator) |Obtient et définit le séparateur de caractères du fichier texte.|
| [separator_string](/cells/fr/python-net/aspose.cells/txtloadoptions/separator_string) | Obtient et définit une valeur de chaîne comme séparateur.|
| [is_multi_encoded](/cells/fr/python-net/aspose.cells/txtloadoptions/is_multi_encoded) | True signifie que le fichier contient plusieurs encodages.|
| [preferred_parsers](/cells/fr/python-net/aspose.cells/txtloadoptions/preferred_parsers) | Obtient et définit les analyseurs de valeur préférés pour le chargement du fichier texte.|
| [has_formula](/cells/fr/python-net/aspose.cells/txtloadoptions/has_formula) | Indique si le texte est une formule s'il commence par "=".|
| [has_text_qualifier](/cells/fr/python-net/aspose.cells/txtloadoptions/has_text_qualifier) | Indique s'il existe un qualificateur de texte pour la valeur de la cellule. La valeur par défaut est true.|
| [text_qualifier](/cells/fr/python-net/aspose.cells/txtloadoptions/text_qualifier) | Spécifie le qualificateur de texte pour les valeurs de cellule. Le qualificateur par défaut est '"'.|
| [treat_consecutive_delimiters_as_one](/cells/fr/python-net/aspose.cells/txtloadoptions/treat_consecutive_delimiters_as_one) |Indique si les délimiteurs consécutifs doivent être traités comme un seul.|
| [treat_quote_prefix_as_value](/cells/fr/python-net/aspose.cells/txtloadoptions/treat_quote_prefix_as_value) |Indique si le guillemet simple de début doit être considéré comme faisant partie de la valeur d'une cellule.<br/>La valeur par défaut est true. S'il est faux, le premier guillemet simple sera supprimé de la valeur de la cellule correspondante<br/> et [Style.quote_prefix](/cells/fr/python-net/aspose.cells/style#quote_prefix) seront définis comme vrais pour la cellule.|
| [extend_to_next_sheet](/cells/fr/python-net/aspose.cells/txtloadoptions/extend_to_next_sheet) | Étend ou non les données à la feuille suivante lorsque les lignes ou les colonnes de données dépassent la limite.<br/>Si cette propriété est vraie, les données supplémentaires seront étendues à la feuille suivante derrière la feuille actuelle (si la feuille actuelle est la dernière,<br/>nouvelle feuille sera ajoutée au classeur actuel).<br/>Si cette propriété est fausse, les données dépassant la limite seront ignorées.<br/> La valeur par défaut est false ;|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [set_paper_size(type)](/cells/fr/python-net/aspose.cells/txtloadoptions/set_paper_size/#PaperSizeType) | Définit le format de papier d'impression par défaut à partir des paramètres par défaut de l'imprimante.|



###  Voir également
* module [aspose.cells](..)
* classe [AbstractTextLoadOptions](/cells/fr/python-net/aspose.cells/abstracttextloadoptions)
* classe [LoadOptions](/cells/fr/python-net/aspose.cells/loadoptions)
* classe [TxtLoadOptions](/cells/fr/python-net/aspose.cells/txtloadoptions)
* classe [Workbook](/cells/fr/python-net/aspose.cells/workbook)
