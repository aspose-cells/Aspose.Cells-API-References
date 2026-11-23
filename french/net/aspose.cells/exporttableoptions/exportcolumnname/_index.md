---
title: "ExportTableOptions.ExportColumnName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExportTableOptions. Indique si les données de la première ligne sont exportées vers le nom de colonne du DataTable. La valeur par défaut est false."
type: docs
url: /fr/net/aspose.cells/exporttableoptions/exportcolumnname/
---
## ExportTableOptions.ExportColumnName property

Indique si les données de la première ligne sont exportées vers le nom de colonne du DataTable. La valeur par défaut est false.

```csharp
public bool ExportColumnName { get; set; }
```

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyExportColumnNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Créer des données d'exemple dans la feuille de calcul
            cells["A1"].PutValue("Column1");
            cells["B1"].PutValue("Column2");
            cells["A2"].PutValue(100);
            cells["B2"].PutValue("Data1");
            cells["A3"].PutValue(200);
            cells["B3"].PutValue("Data2");

            // Configurer les options d'exportation
            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = true; // Demonstrating ExportColumnName property
            options.IsVertical = true;
            options.Indexes = new int[] { 0, 1 }; // Export all columns

            // Exporter les données de la feuille de calcul vers le DataTable
            DataTable dataTable = cells.ExportDataTable(0, 0, 4, 2, options);

            // Affichez les données exportées
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine($"{row["Column1"]}, {row["Column2"]}");
            }
        }
    }
}
```

### Voir aussi

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


