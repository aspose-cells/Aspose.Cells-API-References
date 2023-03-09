---
title: NumbersLoadOptions classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 10
url: /fr/python-net/aspose.cells.numbers/numbersloadoptions/
is_root: false
---
##  NumbersLoadOptions classe
Représente les options de chargement des fichiers Apple Numbers.



**Héritage:** [NumbersLoadOptions](/cells/python-net/aspose.cells.numbers/numbersloadoptions) → 
[LoadOptions](/cells/fr/python-net/aspose.cells/loadoptions)



Le type NumbersLoadOptions expose les membres suivants :

###  Constructeurs
| Constructeur| Description|
| :- | :- |
| [NumbersLoadOptions()](/cells/fr/python-net/aspose.cells.numbers/numbersloadoptions/__init__/#) | Constructeur.|


###  Propriétés
| Propriété| Description|
| :- | :- |
| [load_format](/cells/fr/python-net/aspose.cells.numbers/numbersloadoptions/load_format) | Obtient le format de chargement.|
| [password](/cells/fr/python-net/aspose.cells.numbers/numbersloadoptions/password) | Obtient et définit le mot de passe du classeur.|
| [parsing_formula_on_open](/cells/fr/python-net/aspose.cells.numbers/numbersloadoptions/parsing_formula_on_open) | Indique si l'analyse de la formule lors de la lecture du fichier.|
| [parsing_pivot_cached_records](/cells/fr/python-net/aspose.cells.numbers/numbersloadoptions/parsing_pivot_cached_records) | Indique si l'analyse du pivot a mis en cache les enregistrements lors du chargement du fichier.<br/> La valeur par défaut est faux.|
| [language_code](/cells/fr/python-net/aspose.cells.numbers/numbersloadoptions/language_code) | Obtient ou définit la langue de l'interface utilisateur de la version de Workbook basée sur CountryCode qui a enregistré le fichier.|
| [region](/cells/fr/python-net/aspose.cells.numbers/numbersloadoptions/region) | Obtient ou définit les paramètres régionaux du système en fonction de CountryCode au moment du chargement du fichier.|
| [default_style_settings](/cells/fr/python-net/aspose.cells.numbers/numbersloadoptions/default_style_settings) | Obtient les paramètres de style par défaut pour initialiser les styles du classeur|
| [standard_font](/cells/fr/python-net/aspose.cells.numbers/numbersloadoptions/standard_font) | Définit le nom de police standard par défaut|
| [standard_font_size](/cells/fr/python-net/aspose.cells.numbers/numbersloadoptions/standard_font_size) | Définit la taille de police standard par défaut.|
| [interrupt_monitor](/cells/fr/python-net/aspose.cells.numbers/numbersloadoptions/interrupt_monitor) | Obtient et définit le moniteur d'interruption.|
| [ignore_not_printed](/cells/fr/python-net/aspose.cells.numbers/numbersloadoptions/ignore_not_printed) | Ignorer les données qui ne sont pas imprimées en cas d'impression directe du fichier|
| [check_data_valid](/cells/fr/python-net/aspose.cells.numbers/numbersloadoptions/check_data_valid) | Vérifiez si les données sont valides dans le fichier modèle.|
| [check_excel_restriction](/cells/fr/python-net/aspose.cells.numbers/numbersloadoptions/check_excel_restriction) | Si vérifier la restriction du fichier Excel lorsque l'utilisateur modifie les objets liés aux cellules.<br/>Par exemple, Excel n'autorise pas la saisie d'une valeur de chaîne supérieure à 32 Ko.<br/>Lorsque vous saisissez une valeur supérieure à 32 Ko, par exemple Cell.PutValue(string), si cette propriété est vraie, vous obtiendrez une exception.<br/>Si cette propriété est fausse, nous accepterons votre valeur de chaîne d'entrée comme valeur de la cellule afin que plus tard<br/>vous pouvez générer la valeur de chaîne complète pour d'autres formats de fichier tels que CSV.<br/>Cependant, si vous avez défini un type de valeur non valide pour le format de fichier Excel,<br/> vous ne devez pas enregistrer le classeur au format de fichier Excel ultérieurement. Sinon, il peut y avoir une erreur inattendue pour le fichier Excel généré.|
| [keep_unparsed_data](/cells/fr/python-net/aspose.cells.numbers/numbersloadoptions/keep_unparsed_data) |Indique si les données non analysées sont conservées en mémoire pour le classeur lorsqu'il est chargé à partir du fichier de modèle. La valeur par défaut est true.|
| [load_filter](/cells/fr/python-net/aspose.cells.numbers/numbersloadoptions/load_filter) | Le filtre pour indiquer comment charger les données.|
| [light_cells_data_handler](/cells/fr/python-net/aspose.cells.numbers/numbersloadoptions/light_cells_data_handler) | Le gestionnaire de données pour le traitement des données des cellules lors de la lecture du fichier de modèle.|
| [memory_setting](/cells/fr/python-net/aspose.cells.numbers/numbersloadoptions/memory_setting) | Obtient ou définit les options d'utilisation de la mémoire.|
| [warning_callback](/cells/fr/python-net/aspose.cells.numbers/numbersloadoptions/warning_callback) | Obtient ou définit un rappel d'avertissement.|
| [auto_fitter_options](/cells/fr/python-net/aspose.cells.numbers/numbersloadoptions/auto_fitter_options) | Obtient et définit les options d'ajustement automatique|
| [auto_filter](/cells/fr/python-net/aspose.cells.numbers/numbersloadoptions/auto_filter) | Indique si le filtrage automatique des données lors du chargement des fichiers.|
| [font_configs](/cells/fr/python-net/aspose.cells.numbers/numbersloadoptions/font_configs) | Obtient et définit des configurations de police individuelles.<br/> Ne fonctionne que pour le [Workbook](/cells/fr/python-net/aspose.cells/workbook) qui utilise ce [LoadOptions](/cells/fr/python-net/aspose.cells/loadoptions) pour charger.|
| [load_table_type](/cells/fr/python-net/aspose.cells.numbers/numbersloadoptions/load_table_type) | Obtient et définit le type de chargement de plusieurs tables dans une feuille de calcul.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [set_paper_size(type)](/cells/fr/python-net/aspose.cells.numbers/numbersloadoptions/set_paper_size/#PaperSizeType) | Définit le format de papier d'impression par défaut à partir des paramètres par défaut de l'imprimante.|



###  Voir également
* module [aspose.cells.numbers](..)
* classe [LoadOptions](/cells/fr/python-net/aspose.cells/loadoptions)
* classe [NumbersLoadOptions](/cells/fr/python-net/aspose.cells.numbers/numbersloadoptions)
* classe [Workbook](/cells/fr/python-net/aspose.cells/workbook)
