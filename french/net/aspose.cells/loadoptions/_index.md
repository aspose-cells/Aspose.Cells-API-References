---
title: "Classe LoadOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.LoadOptions. Représente les options de chargement du fichier"
type: docs
url: /fr/net/aspose.cells/loadoptions/
---
## LoadOptions class

Représente les options de chargement du fichier.

```csharp
public class LoadOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [LoadOptions](loadoptions/#constructor)() | Crée une option de chargement du fichier. |
| [LoadOptions](loadoptions/#constructor_1)(LoadFormat) | Crée une option de chargement du fichier. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Indique si le filtrage automatique des données est appliqué lors du chargement des fichiers. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Obtient et définit les options d'ajustement automatique |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Vérifier si les données sont valides dans le fichier modèle. |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Indique si la restriction du fichier Excel est vérifiée lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, par exemple avec Cell.PutValue(string), si cette propriété est vraie, vous obtiendrez une Exception. Si cette propriété est fausse, nous accepterons votre chaîne d'entrée comme valeur de la cellule, de sorte que vous puissiez ensuite exporter la chaîne complète vers d'autres formats de fichier tels que CSV. Cependant, si vous avez défini une valeur qui n'est pas valide pour le format de fichier Excel, vous ne devez pas enregistrer le classeur au format Excel ultérieurement. Sinon, des erreurs inattendues peuvent survenir dans le fichier Excel généré. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Obtient ou définit les paramètres régionaux utilisés pour le classeur qui sera chargé. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Obtient les paramètres de style par défaut pour initialiser les styles du classeur |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Obtient et définit les configurations de police individuelles. Ne fonctionne que pour le [`Workbook`](../workbook/) qui utilise ce `LoadOptions` pour charger. |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignore les données qui ne sont pas imprimées lors de l'impression directe du fichier |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Indique s'il faut ignorer les formes inutiles. |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Obtient et définit le moniteur d'interruption. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Indique s'il faut conserver les données non analysées en mémoire pour le Workbook lorsqu'il est chargé à partir d'un fichier modèle. La valeur par défaut est vraie. |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Obtient ou définit la langue de l'interface utilisateur de la version du classeur basée sur le CountryCode qui a enregistré le fichier. |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Le gestionnaire de données pour le traitement des données des cellules lors de la lecture du fichier modèle. |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Le filtre indiquant comment charger les données. |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Obtient le format de chargement. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Obtient ou définit le mode mémoire pour le classeur chargé. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Indique s'il faut analyser la formule lors de la lecture du fichier. |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Indique s'il faut analyser les enregistrements mis en cache du tableau croisé dynamique lors du chargement du fichier. La valeur par défaut est false. |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Obtient et définit le mot de passe du classeur. |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Indique s'il faut conserver les espaces et les sauts de ligne qui sont insérés entre les jetons de formule lors de l'obtention et de la définition des formules. La valeur par défaut est false. |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Obtient ou définit les paramètres régionaux utilisés pour le classeur qui sera chargé. |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) Définit le nom de police standard par défaut |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) Définit la taille de police standard par défaut. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | Obtient ou définit le rappel d'avertissement. |

## Méthodes

| Nom | Description |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | Définit la taille de papier d'impression par défaut à partir des paramètres de l'imprimante par défaut. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Globalization;

    public class LoadOptionsDemo
    {
        public static void LoadOptionsExample()
        {
            // Créez une instance de LoadOptions
            LoadOptions loadOptions = new LoadOptions();

            // Définition des propriétés
            loadOptions.Password = "password123";
            loadOptions.ParsingFormulaOnOpen = true;
            loadOptions.ParsingPivotCachedRecords = false;
            loadOptions.LanguageCode = CountryCode.USA;
            loadOptions.Region = CountryCode.USA;
            loadOptions.CultureInfo = new CultureInfo("en-US");
            loadOptions.IgnoreNotPrinted = true;
            loadOptions.CheckDataValid = true;
            loadOptions.CheckExcelRestriction = false;
            loadOptions.KeepUnparsedData = true;
            loadOptions.MemorySetting = MemorySetting.MemoryPreference;
            loadOptions.AutoFitterOptions = new AutoFitterOptions { AutoFitMergedCells = true };
            loadOptions.AutoFilter = true;
            loadOptions.IgnoreUselessShapes = true;
            loadOptions.PreservePaddingSpacesInFormula = false;

            // Charger un classeur avec les LoadOptions spécifiés
            Workbook workbook = new Workbook("LoadOptionsExample_original.xlsx", loadOptions);

            // Effectuez des opérations sur le classeur
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello, World!");

            // Enregistrez le classeur
            workbook.Save("LoadOptionsExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


