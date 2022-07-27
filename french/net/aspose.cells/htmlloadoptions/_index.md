---
title: HtmlLoadOptions
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente les options lors de limportation dun fichier html.
type: docs
weight: 3730
url: /fr/net/aspose.cells/htmlloadoptions/
---
## HtmlLoadOptions class

Représente les options lors de l'importation d'un fichier html.

```csharp
public class HtmlLoadOptions : AbstractTextLoadOptions
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [HtmlLoadOptions](htmlloadoptions#constructor)() | Crée une option de chargement du fichier. |
| [HtmlLoadOptions](htmlloadoptions#constructor_1)(LoadFormat) | Crée une option de chargement du fichier. |

## Propriétés

| Nom | La description |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter) { get; set; } | Indique si le filtrage automatique des données lors du chargement des fichiers. |
| [AutoFitColsAndRows](../../aspose.cells/htmlloadoptions/autofitcolsandrows) { get; set; } | Indique si les colonnes et les lignes s'ajustent automatiquement. La valeur par défaut est false. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions) { get; set; } | Obtient et définit les options d'ajustement automatique |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid) { get; set; } | Vérifiez si les données sont valides dans le fichier modèle. |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction) { get; set; } | Vérifier si la restriction du fichier Excel lorsque l'utilisateur modifie les objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une valeur de chaîne supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, comme par Cell.PutValue (chaîne), si cela propriété est vraie, vous obtiendrez une exception. Si cette propriété est fausse, nous accepterons votre valeur de chaîne d'entrée comme valeur de la cellule afin que plus tard vous puissiez sortir la valeur de chaîne complète pour d'autres formats de fichiers tels que CSV. Cependant, si vous avez défini un type de valeur non valide pour le format de fichier Excel, vous ne devez pas enregistrer le classeur au format de fichier Excel ultérieurement. Sinon, il peut y avoir une erreur inattendue pour le fichier Excel généré. |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata) { get; set; } | Obtient ou définit une valeur qui indique si la chaîne dans le fichier texte est convertie en données de date. |
| [ConvertFormulasData](../../aspose.cells/htmlloadoptions/convertformulasdata) { get; set; } | si vrai, convertir la chaîne en formule lorsque la valeur de la chaîne commence par le caractère '=', la valeur par défaut est false. |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata) { get; set; } | Obtient ou définit une valeur qui indique si la chaîne dans le fichier texte est convertie en données numériques. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo) { get; set; } | Obtient ou définit les informations de culture système au moment où le fichier a été chargé. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings) { get; } | Obtient les paramètres de style par défaut pour initialiser les styles du classeur |
| [DeleteRedundantSpaces](../../aspose.cells/htmlloadoptions/deleteredundantspaces) { get; set; } | Indique si les espaces redondants sont supprimés lorsque le texte retourne à la ligne à l'aide de la balise &lt;br&gt;. La valeur par défaut est false. |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding) { get; set; } | Obtient et définit l'encodage par défaut. S'applique uniquement au fichier csv. |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs) { get; set; } | Obtient et définit des configurations de police individuelles. Ne fonctionne que pour le[`Workbook`](../workbook) qui utilise ce[`LoadOptions`](../loadoptions) à charger.&gt; |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted) { get; set; } | Ignorer les données qui ne sont pas imprimées si impression directe du fichier |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor) { get; set; } | Obtient et définit le moniteur d'interruption. |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision) { get; set; } | Indique si une valeur de chaîne n'est pas analysée si la longueur est de 15. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata) { get; set; } | Indique si les données non analysées sont conservées en mémoire pour le classeur lorsqu'il est chargé à partir du fichier de modèle. La valeur par défaut est true. |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode) { get; set; } | Obtient ou définit la langue de l'interface utilisateur de la version du classeur en fonction du code pays qui a enregistré le fichier. |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler) { get; set; } | Le gestionnaire de données pour le traitement des données des cellules lors de la lecture du fichier modèle. |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter) { get; set; } | Le filtre pour indiquer comment charger les données. |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat) { get; } | Obtient le format de chargement. |
| [LoadFormulas](../../aspose.cells/htmlloadoptions/loadformulas) { get; set; } | Indique si les formules sont importées si le fichier html d'origine contient des formules |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy) { get; set; } | Indique la stratégie pour appliquer le style aux valeurs analysées lors de la conversion d'une valeur de chaîne en nombre ou en date/heure. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting) { get; set; } | Obtient ou définit les options d'utilisation de la mémoire. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen) { get; set; } | Indique si l'analyse de la formule lors de la lecture du fichier. |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords) { get; set; } | Indique si l'analyse des enregistrements en cache pivot lors du chargement du fichier. La valeur par défaut est false. |
| [Password](../../aspose.cells/loadoptions/password) { get; set; } | Obtient et définit le mot de passe du classeur. |
| [ProgId](../../aspose.cells/htmlloadoptions/progid) { get; } | Obtient l'ID du programme de création du fichier. Uniquement pour les fichiers MHT. |
| [Region](../../aspose.cells/loadoptions/region) { get; set; } | Obtient ou définit les paramètres régionaux du système en fonction de CountryCode au moment du chargement du fichier. |
| [StreamProvider](../../aspose.cells/htmlloadoptions/streamprovider) { get; set; } | Obtient ou définit le StreamProviderImportHtmlFile pour l'importation d'objets. |
| [SupportDivTag](../../aspose.cells/htmlloadoptions/supportdivtag) { get; set; } | Indique si la disposition de la balise &lt;div&gt; est prise en charge lorsque le fichier html contient des balises &lt;div&gt;. La valeur par défaut est false. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback) { get; set; } | Obtient ou définit un rappel d'avertissement. |

## Méthodes

| Nom | La description |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize)(PaperSizeType) | Définit le format de papier d'impression par défaut à partir des paramètres par défaut de l'imprimante. |

### Voir également

* class [AbstractTextLoadOptions](../abstracttextloadoptions)
* espace de noms [Aspose.Cells](../../aspose.cells)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
