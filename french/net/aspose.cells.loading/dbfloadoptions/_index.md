---
title: "Classe DbfLoadOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Loading.DbfLoadOptions. Représente les options de chargement du fichier .dbf"
type: docs
url: /fr/net/aspose.cells.loading/dbfloadoptions/
---
## DbfLoadOptions class

Représente les options de chargement du fichier .dbf.

```csharp
public class DbfLoadOptions : LoadOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [DbfLoadOptions](dbfloadoptions/)() | Les options. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Indique si le filtrage automatique des données lors du chargement des fichiers. (Hérité de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Obtient et définit les options de l'ajustement automatique (Hérité de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Vérifie si les données sont valides dans le fichier modèle. (Hérité de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Indique si la restriction du fichier Excel est vérifiée lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, par exemple avec Cell.PutValue(string), si cette propriété est vraie, une exception sera levée. Si cette propriété est fausse, nous accepterons votre chaîne d'entrée comme valeur de la cellule, de sorte que vous puissiez ensuite exporter la chaîne complète vers d'autres formats de fichier tels que CSV. Cependant, si vous avez défini une telle valeur qui n'est pas valide pour le format de fichier Excel, vous ne devez pas enregistrer le classeur au format Excel ultérieurement. Sinon, des erreurs inattendues peuvent survenir dans le fichier Excel généré. (Hérité de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Obtient ou définit les paramètres régionaux utilisés pour le Workbook qui sera chargé.(Hérité de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Obtient les paramètres de style par défaut pour l'initialisation des styles du workbook(Hérité de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Obtient et définit les configurations de police individuelles. Fonctionne uniquement pour le [`Workbook`](../../aspose.cells/workbook/) qui utilise ce [`LoadOptions`](../../aspose.cells/loadoptions/) pour charger.(Hérité de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignore les données qui ne sont pas imprimées si le fichier est imprimé directement(Hérité de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Indique s'il faut ignorer les formes inutiles.(Hérité de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Obtient et définit le moniteur d'interruption.(Hérité de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Indique s'il faut conserver les données non analysées en mémoire pour le Workbook lorsqu'il est chargé à partir d'un fichier modèle. La valeur par défaut est true.(Hérité de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Obtient ou définit la langue de l'interface utilisateur de la version du Workbook basée sur le CountryCode qui a enregistré le fichier.(Hérité de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Le gestionnaire de données pour le traitement des données des cellules lors de la lecture du fichier modèle.(Hérité de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Le filtre indiquant comment charger les données.(Hérité de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Obtient le format de chargement.(Hérité de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Obtient ou définit le mode mémoire pour le workbook chargé.(Hérité de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Indique s'il faut analyser la formule lors de la lecture du fichier.(Hérité de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Indique s'il faut analyser les enregistrements mis en cache du tableau croisé dynamique lors du chargement du fichier. La valeur par défaut est false.(Hérité de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Obtient et définit le mot de passe du workbook.(Hérité de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Indique s'il faut conserver les espaces et les sauts de ligne insérés entre les jetons de formule lors de l'obtention et de la définition des formules. La valeur par défaut est false.(Hérité de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Obtient ou définit les paramètres régionaux utilisés pour le Workbook qui sera chargé.(Hérité de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolète.**) Définit le nom de police standard par défaut(Hérité de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolète.**) Définit la taille de police standard par défaut.(Hérité de [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | Obtient ou définit le rappel d'avertissement.(Hérité de [`LoadOptions`](../../aspose.cells/loadoptions/).) |

## Méthodes

| Nom | Description |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | Définit la taille de papier d'impression par défaut à partir des paramètres de l'imprimante par défaut.(Hérité de [`LoadOptions`](../../aspose.cells/loadoptions/).) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Loading;

    public class LoadingClassDbfLoadOptionsDemo
    {
        public static void Run()
        {
            // Créer une instance de DbfLoadOptions
            DbfLoadOptions loadOptions = new DbfLoadOptions();

            // Créer un classeur avec les options de chargement DBF
            Workbook workbook = new Workbook("sample.dbf", loadOptions);

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Modifier certaines cellules (démontrant l'intégration avec d'autres composants)
            worksheet.Cells["A1"].PutValue("Modified DBF Data");
            
            // Enregistrer le classeur au format Excel
            workbook.Save("DbfLoadOptionsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [LoadOptions](../../aspose.cells/loadoptions/)
* namespace [Aspose.Cells.Loading](../../aspose.cells.loading/)
* assembly [Aspose.Cells](../../)


