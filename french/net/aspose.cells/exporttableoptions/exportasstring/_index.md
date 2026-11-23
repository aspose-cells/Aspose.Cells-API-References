---
title: "ExportTableOptions.ExportAsString"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExportTableOptions. Exporte la valeur chaîne des cellules vers le DataTable"
type: docs
url: /fr/net/aspose.cells/exporttableoptions/exportasstring/
---
## ExportTableOptions.ExportAsString property

Exporte la valeur de chaîne des cellules vers le DataTable.

```csharp
public bool ExportAsString { get; set; }
```

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple avec des types mixtes
            worksheet.Cells[0, 0].PutValue("ID");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue(1);
            worksheet.Cells[1, 1].PutValue(123.45);
            worksheet.Cells[2, 0].PutValue(2);
            worksheet.Cells[2, 1].PutValue("TextValue");

            // Créer des options d'exportation avec ExportAsString défini sur true
            ExportTableOptions exportOptions = new ExportTableOptions
            {
                ExportColumnName = true,
                ExportAsString = true // This forces all values to be exported as strings
            };

            // Exporter les données vers DataTable
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 3, 2, exportOptions);

            // Afficher les types de données exportés
            Console.WriteLine("Data exported with ExportAsString=true:");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine($"{row[0]} ({row[0].GetType().Name}) | {row[1]} ({row[1].GetType().Name})");
            }

            // Exporter maintenant avec ExportAsString=false
            exportOptions.ExportAsString = false;
            DataTable dataTable2 = worksheet.Cells.ExportDataTable(0, 0, 3, 2, exportOptions);

            Console.WriteLine("\nData exported with ExportAsString=false:");
            foreach (DataRow row in dataTable2.Rows)
            {
                Console.WriteLine($"{row[0]} ({row[0].GetType().Name}) | {row[1]} ({row[1].GetType().Name})");
            }
        }
    }
}
```

### Voir aussi

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


