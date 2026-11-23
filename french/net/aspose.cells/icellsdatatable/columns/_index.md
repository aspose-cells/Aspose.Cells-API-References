---
title: "ICellsDataTable.Columns"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ICellsDataTable. Obtient le nom des colonnes"
type: docs
url: /fr/net/aspose.cells/icellsdatatable/columns/
---
## ICellsDataTable.Columns property

Obtient le nom des colonnes.

```csharp
public string[] Columns { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICellsDataTablePropertyColumnsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des données d'exemple
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["C1"].PutValue("Stock");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);
            worksheet.Cells["C2"].PutValue(15);

            try
            {
                // Exporter la plage de données vers ICellsDataTable
                ICellsDataTable dataTable = (ICellsDataTable)worksheet.Cells.ExportDataTable(0, 0, 2, 3);

                // Afficher les noms des colonnes
                Console.WriteLine("Column names in the data table:");
                foreach (string column in dataTable.Columns)
                {
                    Console.WriteLine(column);
                }

                // Afficher le nombre de colonnes
                Console.WriteLine($"Total columns: {dataTable.Columns.Length}");

                // Enregistrez le classeur
                workbook.Save("ColumnsDemo.xlsx");
                Console.WriteLine("Columns property demonstrated successfully.");
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

* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


