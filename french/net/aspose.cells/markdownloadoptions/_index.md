---
title: "Class MarkdownLoadOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.MarkdownLoadOptions. Représente les options de chargement du document markdown"
type: docs
url: /fr/net/aspose.cells/markdownloadoptions/
---
## MarkdownLoadOptions class

Représente les options de chargement du document markdown.

```csharp
public class MarkdownLoadOptions : AbstractTextLoadOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [MarkdownLoadOptions](markdownloadoptions/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Indique si le filtrage automatique des données lors du chargement des fichiers est activé. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Obtient et définit les options d'ajustement automatique (Hérité de [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Vérifie si les données sont valides dans le fichier modèle. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Indique si la restriction du fichier Excel est vérifiée lorsque l'utilisateur modifie des objets liés aux cellules. Par exemple, Excel n'autorise pas la saisie d'une chaîne de caractères supérieure à 32 K. Lorsque vous saisissez une valeur supérieure à 32 K, par exemple avec Cell.PutValue(string), si cette propriété est vraie, vous obtiendrez une exception. Si cette propriété est fausse, nous accepterons votre chaîne saisie comme valeur de la cellule, de sorte que vous puissiez ensuite exporter la chaîne complète vers d'autres formats de fichier tels que CSV. Cependant, si vous avez défini une valeur qui n'est pas valide pour le format de fichier Excel, vous ne devez pas enregistrer le classeur au format Excel ultérieurement. Sinon, il peut y avoir des erreurs inattendues dans le fichier Excel généré. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata/) { get; set; } | Obtient ou définit une valeur qui indique si la chaîne du fichier texte est convertie en données de date. La valeur par défaut est true.(Hérité de [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata/) { get; set; } | Obtient ou définit une valeur qui indique si la chaîne du fichier texte est convertie en données numériques. La valeur par défaut est true.(Hérité de [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Obtient ou définit les paramètres régionaux utilisés pour le classeur qui sera chargé. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Obtient les paramètres de style par défaut pour l'initialisation des styles du classeur (Hérité de [`LoadOptions`](../loadoptions/).) |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding/) { get; set; } | Obtient et définit l'encodage par défaut. S'applique uniquement aux fichiers csv.(Hérité de [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Obtient et définit les configurations de police individuelles. Ne fonctionne que pour le [`Workbook`](../workbook/) qui utilise ce [`LoadOptions`](../loadoptions/) pour le chargement. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [HasFormula](../../aspose.cells/markdownloadoptions/hasformula/) { get; set; } | Indique si le texte est une formule lorsqu'il commence par "=". |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignore les données qui ne sont pas imprimées lors de l'impression directe du fichier (Hérité de [`LoadOptions`](../loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Indique s'il faut ignorer les formes inutiles. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Obtient et définit le moniteur d'interruption. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision/) { get; set; } | Indique s'il ne faut pas analyser une valeur de chaîne si sa longueur est de 15.(Hérité de [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Indique s'il faut conserver les données non analysées en mémoire pour le classeur lorsqu'il est chargé à partir d'un fichier modèle. La valeur par défaut est vraie. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Obtient ou définit la langue de l'interface utilisateur de la version du classeur basée sur le CountryCode qui a enregistré le fichier. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Le gestionnaire de données pour le traitement des données des cellules lors de la lecture du fichier modèle. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Le filtre indiquant comment charger les données. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Obtient le format de chargement. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy/) { get; set; } | Indique la stratégie à appliquer pour le style des valeurs analysées lors de la conversion d'une valeur chaîne en nombre ou date/heure.(Hérité de [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Obtient ou définit le mode mémoire pour le classeur chargé. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Indique s'il faut analyser la formule lors de la lecture du fichier. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Indique s'il faut analyser les enregistrements en cache du tableau croisé dynamique lors du chargement du fichier. La valeur par défaut est false. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Obtient et définit le mot de passe du classeur. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Indique si l'on doit préserver ces espaces et sauts de ligne qui sont remplis entre les jetons de formule lors de la récupération et de la définition des formules. La valeur par défaut est false.(Hérité de [`LoadOptions`](../loadoptions/).) |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Obtient ou définit les paramètres régionaux utilisés pour le classeur qui sera chargé. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) Définit le nom de police standard par défaut (Hérité de [`LoadOptions`](../loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) Définit la taille de police standard par défaut. (Hérité de [`LoadOptions`](../loadoptions/).) |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | Obtient ou définit le rappel d'avertissement. (Hérité de [`LoadOptions`](../loadoptions/).) |

## Méthodes

| Nom | Description |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | Définit la taille de papier d'impression par défaut à partir des paramètres de l'imprimante par défaut. (Hérité de [`LoadOptions`](../loadoptions/).) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassMarkdownLoadOptionsDemo
    {
        public static void Run()
        {
            try
            {
                // Créer une instance de MarkdownLoadOptions
                MarkdownLoadOptions options = new MarkdownLoadOptions();

                // Définir la propriété HasFormula
                options.HasFormula = true;

                // Afficher la valeur de la propriété
                Console.WriteLine($"HasFormula property is set to: {options.HasFormula}");

                // Créer un classeur et charger un fichier markdown avec les options
                Workbook workbook = new Workbook("sample.md", options);

                // Enregistrer le classeur au format Excel
                workbook.Save("output.xlsx");

                Console.WriteLine("Markdown file loaded and converted to Excel successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [AbstractTextLoadOptions](../abstracttextloadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


