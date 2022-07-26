---
title: TxtLoadOptions
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente les options de chargement du fichier texte.
type: docs
weight: 6110
url: /fr/net/aspose.cells/txtloadoptions/
---
## TxtLoadOptions class

Représente les options de chargement du fichier texte.

```csharp
public class TxtLoadOptions : AbstractTextLoadOptions
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [TxtLoadOptions](txtloadoptions#constructor)() | Crée les options de chargement du fichier texte. |
| [TxtLoadOptions](txtloadoptions#constructor_1)(LoadFormat) | Crée les options de chargement du fichier texte. |

## Propriétés

| Nom | La description |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter) { get; set; } | Indique si le filtrage automatique des données lors du chargement des fichiers. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions) { get; set; } | Obtient et définit les options d'ajustement automatique |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid) { get; set; } | Vérifiez si les données sont valides dans le fichier modèle. |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction) { get; set; } | Vérifier si la restriction du fichier Excel lorsque l'utilisateur modifie les objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une valeur de chaîne supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, comme par Cell.PutValue (chaîne), si cela propriété est vraie, vous obtiendrez une exception. Si cette propriété est fausse, nous accepterons votre valeur de chaîne d'entrée comme valeur de la cellule afin que plus tard vous puissiez sortir la valeur de chaîne complète pour d'autres formats de fichiers tels que CSV. Cependant, si vous avez défini un type de valeur non valide pour le format de fichier Excel, vous ne devez pas enregistrer le classeur au format de fichier Excel ultérieurement. Sinon, il peut y avoir une erreur inattendue pour le fichier Excel généré. |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata) { get; set; } | Obtient ou définit une valeur qui indique si la chaîne dans le fichier texte est convertie en données de date. |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata) { get; set; } | Obtient ou définit une valeur qui indique si la chaîne dans le fichier texte est convertie en données numériques. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo) { get; set; } | Obtient ou définit les informations de culture système au moment où le fichier a été chargé. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings) { get; } | Obtient les paramètres de style par défaut pour initialiser les styles du classeur |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding) { get; set; } | Obtient et définit l'encodage par défaut. S'applique uniquement au fichier csv. |
| [ExtendToNextSheet](../../aspose.cells/txtloadoptions/extendtonextsheet) { get; set; } | Indique si les données sont étendues à la feuille suivante lorsque les lignes ou les colonnes de données dépassent la limite. Si cette propriété est vraie, les données supplémentaires seront étendues à la feuille suivante derrière la feuille actuelle (si la feuille actuelle est la dernière, la nouvelle feuille sera ajoutée au classeur en cours). Si cette propriété est fausse, les données dépassant la limite seront ignorées. La valeur par défaut est fausse ; |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs) { get; set; } | Obtient et définit des configurations de police individuelles. Ne fonctionne que pour le[`Workbook`](../workbook) qui utilise ce[`LoadOptions`](../loadoptions) à charger.&gt; |
| [HasFormula](../../aspose.cells/txtloadoptions/hasformula) { get; set; } | Indique si le texte est une formule s'il commence par "=". |
| [HasTextQualifier](../../aspose.cells/txtloadoptions/hastextqualifier) { get; set; } | Indique s'il existe un qualificateur de texte pour la valeur de la cellule. La valeur par défaut est true. |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted) { get; set; } | Ignorer les données qui ne sont pas imprimées si impression directe du fichier |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor) { get; set; } | Obtient et définit le moniteur d'interruption. |
| [IsMultiEncoded](../../aspose.cells/txtloadoptions/ismultiencoded) { get; set; } | Vrai signifie que le fichier contient plusieurs encodages. |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision) { get; set; } | Indique si une valeur de chaîne n'est pas analysée si la longueur est de 15. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata) { get; set; } | Indique si les données non analysées sont conservées en mémoire pour le classeur lorsqu'il est chargé à partir du fichier de modèle. La valeur par défaut est true. |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode) { get; set; } | Obtient ou définit la langue de l'interface utilisateur de la version du classeur en fonction du code pays qui a enregistré le fichier. |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler) { get; set; } | Le gestionnaire de données pour le traitement des données des cellules lors de la lecture du fichier modèle. |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter) { get; set; } | Le filtre pour indiquer comment charger les données. |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat) { get; } | Obtient le format de chargement. |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy) { get; set; } | Indique la stratégie pour appliquer le style aux valeurs analysées lors de la conversion d'une valeur de chaîne en nombre ou en date/heure. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting) { get; set; } | Obtient ou définit les options d'utilisation de la mémoire. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen) { get; set; } | Indique si l'analyse de la formule lors de la lecture du fichier. |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords) { get; set; } | Indique si l'analyse des enregistrements en cache pivot lors du chargement du fichier. La valeur par défaut est false. |
| [Password](../../aspose.cells/loadoptions/password) { get; set; } | Obtient et définit le mot de passe du classeur. |
| [PreferredParsers](../../aspose.cells/txtloadoptions/preferredparsers) { get; set; } | Obtient et définit les analyseurs de valeurs préférés pour le chargement du fichier texte. |
| [Region](../../aspose.cells/loadoptions/region) { get; set; } | Obtient ou définit les paramètres régionaux du système en fonction de CountryCode au moment du chargement du fichier. |
| [Separator](../../aspose.cells/txtloadoptions/separator) { get; set; } | Obtient et définit le séparateur de caractères du fichier texte. |
| [SeparatorString](../../aspose.cells/txtloadoptions/separatorstring) { get; set; } | Obtient et définit une valeur de chaîne comme séparateur. |
| [TextQualifier](../../aspose.cells/txtloadoptions/textqualifier) { get; set; } | Spécifie le qualificateur de texte pour les valeurs de cellule. Le qualificateur par défaut est '"'. |
| [TreatConsecutiveDelimitersAsOne](../../aspose.cells/txtloadoptions/treatconsecutivedelimitersasone) { get; set; } | Indique si les délimiteurs consécutifs doivent être traités comme un seul. |
| [TreatQuotePrefixAsValue](../../aspose.cells/txtloadoptions/treatquoteprefixasvalue) { get; set; } | Indique si le premier guillemet simple doit être considéré comme faisant partie de la valeur d'une cellule. La valeur par défaut est true. S'il est faux, le guillemet simple de tête sera supprimé de la cellule correspondante value et[`QuotePrefix`](../style/quoteprefix) sera défini comme vrai pour la cellule. |
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
