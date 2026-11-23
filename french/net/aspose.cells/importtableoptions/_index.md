---
title: "Classe ImportTableOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.ImportTableOptions classe. Représente les options d'importation de données dans les cellules"
type: docs
url: /fr/net/aspose.cells/importtableoptions/
---
## ImportTableOptions class

Représente les options d'importation de données dans les cellules.

```csharp
public class ImportTableOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ImportTableOptions](importtableoptions/)() | Crée les options d'importation par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [CheckMergedCells](../../aspose.cells/importtableoptions/checkmergedcells/) { get; set; } | Indique si les cellules fusionnées sont vérifiées. |
| [ColumnIndexes](../../aspose.cells/importtableoptions/columnindexes/) { get; set; } | Obtient ou définit les colonnes (indexées à partir de 0) à importer depuis la source de données. null signifie que toutes les colonnes doivent être importées. |
| [ConvertGridStyle](../../aspose.cells/importtableoptions/convertgridstyle/) { get; set; } | Indique si le style de la vue grille doit être appliqué aux cellules. |
| [ConvertNumericData](../../aspose.cells/importtableoptions/convertnumericdata/) { get; set; } | Obtient ou définit une valeur qui indique si la valeur chaîne doit être convertie en valeur numérique ou date. |
| [DateFormat](../../aspose.cells/importtableoptions/dateformat/) { get; set; } | Obtient ou définit la chaîne de format de date pour les cellules contenant des valeurs datetime importées. |
| [DefaultValues](../../aspose.cells/importtableoptions/defaultvalues/) { get; set; } | La valeur par défaut pour la valeur dans le tableau est null. |
| [ExportCaptionAsFieldName](../../aspose.cells/importtableoptions/exportcaptionasfieldname/) { get; set; } | Indique si la légende est exportée comme nom de champ |
| [InsertRows](../../aspose.cells/importtableoptions/insertrows/) { get; set; } | Indique si de nouvelles lignes doivent être ajoutées pour l'importation des enregistrements de données. |
| [IsFieldNameShown](../../aspose.cells/importtableoptions/isfieldnameshown/) { get; set; } | Indique si le nom du champ doit être importé. |
| [IsFormulas](../../aspose.cells/importtableoptions/isformulas/) { get; set; } | Indique si les données sont des formules. |
| [IsHtmlString](../../aspose.cells/importtableoptions/ishtmlstring/) { get; set; } | Indique si la valeur contient des balises HTML. |
| [NumberFormats](../../aspose.cells/importtableoptions/numberformats/) { get; set; } | Obtient ou définit les formats numériques |
| [ShiftFirstRowDown](../../aspose.cells/importtableoptions/shiftfirstrowdown/) { get; set; } | Indique si la première ligne doit être décalée vers le bas lors de l'insertion de lignes. |
| [Styles](../../aspose.cells/importtableoptions/styles/) { get; set; } | Obtient et définit les styles pour chaque colonne du tableau. |
| [TotalColumns](../../aspose.cells/importtableoptions/totalcolumns/) { get; set; } | Obtient ou définit le nombre total de colonnes à importer depuis la source de données. -1 signifie que toutes les lignes de la source de données donnée. |
| [TotalRows](../../aspose.cells/importtableoptions/totalrows/) { get; set; } | Obtient ou définit le nombre total de lignes à importer depuis la source de données. -1 signifie que toutes les lignes de la source de données donnée. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ImportTableOptionsDemo
    {
        public static void ImportTableOptionsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez un DataTable à importer
            DataTable dataTable = new DataTable("SampleData");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Date", typeof(DateTime));
            dataTable.Rows.Add(1, "John Doe", DateTime.Now);
            dataTable.Rows.Add(2, "Jane Smith", DateTime.Now.AddDays(1));

            // Créez une instance de ImportTableOptions
            ImportTableOptions importOptions = new ImportTableOptions
            {
                ConvertGridStyle = true,
                ConvertNumericData = true,
                InsertRows = true,
                ShiftFirstRowDown = false,
                IsFieldNameShown = true,
                ExportCaptionAsFieldName = false,
                DateFormat = "yyyy-MM-dd",
                TotalRows = -1, // Import all rows
                TotalColumns = -1, // Import all columns
                IsHtmlString = false,
                CheckMergedCells = false
            };

            // Importer le DataTable dans la feuille de calcul
            worksheet.Cells.ImportData(dataTable, 0, 0, importOptions);

            // Enregistrez le classeur
            workbook.Save("ImportTableOptionsExample.xlsx");
            workbook.Save("ImportTableOptionsExample.pdf");
            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


