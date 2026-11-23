---
title: "ExportTableOptions.AllowDBNull"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExportTableOptions. Cette valeur indique si les DBNull sont autorisés dans cette table"
type: docs
url: /fr/net/aspose.cells/exporttableoptions/allowdbnull/
---
## ExportTableOptions.AllowDBNull property

Cette valeur indique si les DBNull sont autorisés dans ce tableau.

```csharp
public bool AllowDBNull { get; set; }
```

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyAllowDBNullDemo
    {
        public static void Run()
        {
            // Créer un classeur d'exemple avec des données de test
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple avec quelques cellules vides
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue(""); // Empty cell
            worksheet.Cells["B3"].PutValue(25);

            // Exporter avec AllowDBNull = true (par défaut)
            ExportTableOptions options1 = new ExportTableOptions
            {
                ExportColumnName = true,
                AllowDBNull = true
            };
            
            DataTable table1 = worksheet.Cells.ExportDataTable(0, 0, 3, 2, options1);
            Console.WriteLine("With AllowDBNull=true:");
            Console.WriteLine("Row 2 Name: " + (table1.Rows[1]["Name"] == DBNull.Value ? "DBNull" : table1.Rows[1]["Name"]));

            // Exporter avec AllowDBNull = false
            ExportTableOptions options2 = new ExportTableOptions
            {
                ExportColumnName = true,
                AllowDBNull = false
            };
            
            DataTable table2 = worksheet.Cells.ExportDataTable(0, 0, 3, 2, options2);
            Console.WriteLine("\nWith AllowDBNull=false:");
            Console.WriteLine("Row 2 Name: " + (table2.Rows[1]["Name"] == DBNull.Value ? "DBNull" : table2.Rows[1]["Name"]));
        }
    }
}
```

### Voir aussi

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


