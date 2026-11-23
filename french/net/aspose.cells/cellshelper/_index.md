---
title: "Classe CellsHelper"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.CellsHelper. Fournit des fonctions d'assistance"
type: docs
url: /fr/net/aspose.cells/cellshelper/
---
## CellsHelper class

Fournit des fonctions d'assistance.

```csharp
public class CellsHelper
```

## Propriétés

| Nom | Description |
| --- | --- |
| static [AltStartPath](../../aspose.cells/cellshelper/altstartpath/) { get; set; } | Obtient ou définit le chemin de démarrage alternatif, qui est référencé par certaines références de formules externes. |
| static [CustomImplementationFactory](../../aspose.cells/cellshelper/customimplementationfactory/) { get; set; } | Obtient ou définit la fabrique pour créer des instances avec une implémentation spéciale. |
| static [DPI](../../aspose.cells/cellshelper/dpi/) { get; set; } | Obtient le DPI de la machine. |
| static [IsCloudPlatform](../../aspose.cells/cellshelper/iscloudplatform/) { get; set; } | Veuillez définir cette propriété sur True lors de l'exécution sur une plateforme cloud, telle que : Azure, AWSLambda, etc, |
| static [LibraryPath](../../aspose.cells/cellshelper/librarypath/) { get; set; } | Obtient ou définit le chemin de la bibliothèque qui est référencé par certaines références de formules externes. |
| static [SignificantDigits](../../aspose.cells/cellshelper/significantdigits/) { get; set; } | (**Obsolete.**) Obtient et définit le nombre de chiffres significatifs. La valeur par défaut est 17. |
| static [SignificantDigitsType](../../aspose.cells/cellshelper/significantdigitstype/) { get; set; } | Obtient et définit le type par défaut de chiffres significatifs pour la sortie des valeurs numériques. La valeur par défaut est G17. |
| static [StartupPath](../../aspose.cells/cellshelper/startuppath/) { get; set; } | Obtient ou définit le chemin de démarrage, qui est référencé par certaines références de formules externes. |

## Méthodes

| Nom | Description |
| --- | --- |
| static [AddAddInFunction](../../aspose.cells/cellshelper/addaddinfunction/)(string, int, int, ParameterType[], ParameterType) | (**Obsolete.**) Ajoute la fonction d'add-in. |
| static [CellIndexToName](../../aspose.cells/cellshelper/cellindextoname/)(int, int) | Obtient le nom de la cellule selon ses indices de ligne et de colonne. |
| static [CellNameToIndex](../../aspose.cells/cellshelper/cellnametoindex/)(string, out int, out int) | Obtient les indices de ligne et de colonne de la cellule selon son nom. |
| static [ColumnIndexToName](../../aspose.cells/cellshelper/columnindextoname/)(int) | Obtient le nom de la colonne selon l'indice de colonne. |
| static [ColumnNameToIndex](../../aspose.cells/cellshelper/columnnametoindex/)(string) | Obtient l'indice de colonne selon le nom de la colonne. |
| static [ConvertA1FormulaToR1C1](../../aspose.cells/cellshelper/converta1formulator1c1/)(string, int, int) | (**Obsolète.**) Convertit la formule A1 de la cellule en formule r1c1. |
| static [ConvertR1C1FormulaToA1](../../aspose.cells/cellshelper/convertr1c1formulatoa1/)(string, int, int) | (**Obsolète.**) Convertit la formule r1c1 de la cellule en formule A1. |
| static [CreateSafeSheetName](../../aspose.cells/cellshelper/createsafesheetname/#createsafesheetname)(string) | Vérifie le nom de feuille fourni et crée un nom valide si nécessaire. Si le nom de feuille fourni respecte les règles de nommage des feuilles Excel, il est renvoyé. Sinon, la chaîne sera tronquée si sa longueur dépasse la limite et les caractères invalides seront remplacés par ' ', puis la valeur de chaîne reconstruite sera renvoyée. |
| static [CreateSafeSheetName](../../aspose.cells/cellshelper/createsafesheetname/#createsafesheetname_1)(string, char) | Vérifie le nom de feuille fourni et crée un nom valide si nécessaire. Si le nom de feuille fourni respecte les règles de nommage des feuilles Excel, il est renvoyé. Sinon, la chaîne sera tronquée si sa longueur dépasse la limite et les caractères invalides seront remplacés par le caractère fourni, puis la valeur de chaîne reconstruite sera renvoyée. |
| static [GetCacheFolder](../../aspose.cells/cellshelper/getcachefolder/)() | Obtient le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données. |
| static [GetDateTimeFromDouble](../../aspose.cells/cellshelper/getdatetimefromdouble/)(double, bool) | Convertit la valeur double en valeur date‑heure. |
| static [GetDoubleFromDateTime](../../aspose.cells/cellshelper/getdoublefromdatetime/)(DateTime, bool) | Convertit la date‑heure en valeur double. |
| static [GetTextWidth](../../aspose.cells/cellshelper/gettextwidth/)(string, Font, double) | Obtient la largeur du texte en points. |
| static [GetUsedColors](../../aspose.cells/cellshelper/getusedcolors/)(Workbook) | Obtient toutes les couleurs utilisées dans le classeur. |
| static [GetVersion](../../aspose.cells/cellshelper/getversion/)() | Obtient la version de publication. |
| static [MergeFiles](../../aspose.cells/cellshelper/mergefiles/)(string[], string, string) | Fusionne plusieurs gros fichiers xls en un fichier xls. |
| static [NeedQuoteInFormula](../../aspose.cells/cellshelper/needquoteinformula/)(string) | Indique si le nom de la feuille doit être entouré de guillemets simples. |
| static [RowIndexToName](../../aspose.cells/cellshelper/rowindextoname/)(int) | Obtient le nom de la ligne selon l'indice de ligne. |
| static [RowNameToIndex](../../aspose.cells/cellshelper/rownametoindex/)(string) | Obtient l'indice de ligne selon le nom de la ligne. |
| static [SetCacheFolder](../../aspose.cells/cellshelper/setcachefolder/)(string) | Définit le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperDemo
    {
        public static void CellsHelperExample()
        {
            // Définition des propriétés de CellsHelper
            CellsHelper.SignificantDigits = 15;
            CellsHelper.DPI = 96.0;
            CellsHelper.StartupPath = "C:\\Program Files\\Aspose\\Cells";
            CellsHelper.AltStartPath = "D:\\Aspose\\Cells";
            CellsHelper.LibraryPath = "E:\\Aspose\\Cells\\Library";
            CellsHelper.IsCloudPlatform = true;

            // En supposant que CustomImplementationFactory est déjà défini et instancié ailleurs
            CellsHelper.CustomImplementationFactory = new CustomImplementationFactory();

            // Démonstration de l'utilisation des propriétés de CellsHelper
            Console.WriteLine("Significant Digits: " + CellsHelper.SignificantDigits);
            Console.WriteLine("DPI: " + CellsHelper.DPI);
            Console.WriteLine("Startup Path: " + CellsHelper.StartupPath);
            Console.WriteLine("Alternate Startup Path: " + CellsHelper.AltStartPath);
            Console.WriteLine("Library Path: " + CellsHelper.LibraryPath);
            Console.WriteLine("Is Cloud Platform: " + CellsHelper.IsCloudPlatform);

            // Exemple d'utilisation de CustomImplementationFactory
            var memoryStream = CellsHelper.CustomImplementationFactory.CreateMemoryStream();
            Console.WriteLine("MemoryStream created with CustomImplementationFactory: " + (memoryStream != null));

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


