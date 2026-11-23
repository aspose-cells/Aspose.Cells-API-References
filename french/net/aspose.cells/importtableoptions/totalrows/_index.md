---
title: "ImportTableOptions.TotalRows"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImportTableOptions. Obtient ou définit le nombre total de lignes à importer depuis la source de données. 1 signifie toutes les lignes de la source de données donnée"
type: docs
url: /fr/net/aspose.cells/importtableoptions/totalrows/
---
## ImportTableOptions.TotalRows property

Obtient ou définit le nombre total de lignes à importer depuis la source de données. -1 signifie que toutes les lignes de la source de données donnée.

```csharp
public int TotalRows { get; set; }
```

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyTotalRowsDemo
    {
        public static void Run()
        {
            // Créez un DataTable d'exemple
            DataTable table = new DataTable("TestTable");
            table.Columns.Add("Column1", typeof(string));
            table.Columns.Add("Column2", typeof(int));
            
            // Ajoutez des données d'exemple
            table.Rows.Add("Item1", 100);
            table.Rows.Add("Item2", 200);
            table.Rows.Add("Item3", 300);

            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer ImportTableOptions avec TotalRows défini à 2 (importera uniquement les 2 premières lignes)
            ImportTableOptions options = new ImportTableOptions
            {
                IsFieldNameShown = true,
                TotalRows = 2 // Only import 2 rows from the DataTable
            };

            // Importer des données avec les options spécifiées
            worksheet.Cells.ImportData(table, 0, 0, options);

            // Enregistrez le classeur
            workbook.Save("ImportWithTotalRows.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Data imported with TotalRows=2. Only first 2 rows were imported.");
        }
    }
}
```

### Voir aussi

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


