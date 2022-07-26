---
title: OdsLoadOptions
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente les options de chargement du fichier ods.
type: docs
weight: 4330
url: /fr/net/aspose.cells/odsloadoptions/
---
## OdsLoadOptions class

Représente les options de chargement du fichier ods.

```csharp
public class OdsLoadOptions : LoadOptions
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [OdsLoadOptions](odsloadoptions#constructor)() | Représente les options de chargement du fichier ods. |
| [OdsLoadOptions](odsloadoptions#constructor_1)(LoadFormat) | Représente les options de chargement du fichier ods. |

## Propriétés

| Nom | La description |
| --- | --- |
| [ApplyExcelDefaultStyleToHyperlink](../../aspose.cells/odsloadoptions/applyexceldefaultstyletohyperlink) { get; set; } | Indique si le style par défaut d'Excel est appliqué au lien hypertexte. |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter) { get; set; } | Indique si le filtrage automatique des données lors du chargement des fichiers. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions) { get; set; } | Obtient et définit les options d'ajustement automatique |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid) { get; set; } | Vérifiez si les données sont valides dans le fichier modèle. |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction) { get; set; } | Vérifier si la restriction du fichier Excel lorsque l'utilisateur modifie les objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une valeur de chaîne supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, comme par Cell.PutValue (chaîne), si cela propriété est vraie, vous obtiendrez une exception. Si cette propriété est fausse, nous accepterons votre valeur de chaîne d'entrée comme valeur de la cellule afin que plus tard vous puissiez sortir la valeur de chaîne complète pour d'autres formats de fichiers tels que CSV. Cependant, si vous avez défini un type de valeur non valide pour le format de fichier Excel, vous ne devez pas enregistrer le classeur au format de fichier Excel ultérieurement. Sinon, il peut y avoir une erreur inattendue pour le fichier Excel généré. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo) { get; set; } | Obtient ou définit les informations de culture système au moment où le fichier a été chargé. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings) { get; } | Obtient les paramètres de style par défaut pour initialiser les styles du classeur |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs) { get; set; } | Obtient et définit des configurations de police individuelles. Ne fonctionne que pour le[`Workbook`](../workbook) qui utilise ce[`LoadOptions`](../loadoptions) à charger.&gt; |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted) { get; set; } | Ignorer les données qui ne sont pas imprimées si impression directe du fichier |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor) { get; set; } | Obtient et définit le moniteur d'interruption. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata) { get; set; } | Indique si les données non analysées sont conservées en mémoire pour le classeur lorsqu'il est chargé à partir du fichier de modèle. La valeur par défaut est true. |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode) { get; set; } | Obtient ou définit la langue de l'interface utilisateur de la version du classeur en fonction du code pays qui a enregistré le fichier. |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler) { get; set; } | Le gestionnaire de données pour le traitement des données des cellules lors de la lecture du fichier modèle. |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter) { get; set; } | Le filtre pour indiquer comment charger les données. |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat) { get; } | Obtient le format de chargement. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting) { get; set; } | Obtient ou définit les options d'utilisation de la mémoire. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen) { get; set; } | Indique si l'analyse de la formule lors de la lecture du fichier. |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords) { get; set; } | Indique si l'analyse des enregistrements en cache pivot lors du chargement du fichier. La valeur par défaut est false. |
| [Password](../../aspose.cells/loadoptions/password) { get; set; } | Obtient et définit le mot de passe du classeur. |
| [RefreshPivotTables](../../aspose.cells/odsloadoptions/refreshpivottables) { get; set; } | Indique si les tableaux croisés dynamiques sont actualisés lors du chargement du fichier. |
| [Region](../../aspose.cells/loadoptions/region) { get; set; } | Obtient ou définit les paramètres régionaux du système en fonction de CountryCode au moment du chargement du fichier. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback) { get; set; } | Obtient ou définit un rappel d'avertissement. |

## Méthodes

| Nom | La description |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize)(PaperSizeType) | Définit le format de papier d'impression par défaut à partir des paramètres par défaut de l'imprimante. |

### Voir également

* class [LoadOptions](../loadoptions)
* espace de noms [Aspose.Cells](../../aspose.cells)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
