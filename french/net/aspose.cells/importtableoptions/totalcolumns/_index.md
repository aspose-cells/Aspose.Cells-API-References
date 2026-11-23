---
title: "ImportTableOptions.TotalColumns"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImportTableOptions. Obtient ou définit le nombre total de colonnes à importer depuis la source de données. 1 signifie toutes les lignes de la source de données donnée"
type: docs
url: /fr/net/aspose.cells/importtableoptions/totalcolumns/
---
## ImportTableOptions.TotalColumns property

Obtient ou définit le nombre total de colonnes à importer depuis la source de données. -1 signifie que toutes les lignes de la source de données donnée.

```csharp
public int TotalColumns { get; set; }
```

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyTotalColumnsDemo
    {
        public static void Run()
        {
            // Créez un DataTable d'exemple
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            
            // Ajoutez des données d'exemple
            dataTable.Rows.Add(1, "Product A", 19.99m);
            dataTable.Rows.Add(2, "Product B", 29.99m);

            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir les options d'importation avec TotalColumns = 2 (n'importera que les 2 premières colonnes)
            ImportTableOptions importOptions = new ImportTableOptions
            {
                IsFieldNameShown = true,
                TotalColumns = 2 // Only import first 2 columns (ID and Name)
            };

            // Importer des données à partir de la cellule A1
            cells.ImportData(dataTable, 0, 0, importOptions);

            // Enregistrez le classeur
            workbook.Save("ImportWithTotalColumns.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Data imported with TotalColumns=2. Only first 2 columns were imported.");
        }
    }
}
```

### Voir aussi

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


