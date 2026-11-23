---
title: "ExportTableOptions.DataTable"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExportTableOptions. Obtient et définit le DataTable auquel le type de données des colonnes est attribué"
type: docs
url: /fr/net/aspose.cells/exporttableoptions/datatable/
---
## ExportTableOptions.DataTable property

Obtient et définit le DataTable auquel le type de données des colonnes est attribué.

```csharp
public DataTable DataTable { get; set; }
```

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyDataTableDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ajoutez des données d'exemple aux cellules
            cells["A1"].PutValue("Column1");
            cells["B1"].PutValue("Column2");
            cells["A2"].PutValue(100);
            cells["B2"].PutValue("Text1");
            cells["A3"].PutValue(200);
            cells["B3"].PutValue("Text2");

            // Créer un DataTable et définir les colonnes
            DataTable dt = new DataTable();
            dt.Columns.Add("NumericData", typeof(double));
            dt.Columns.Add("TextData", typeof(string));

            // Configurer les options d'exportation
            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = true;
            options.Indexes = new int[] { 0, 1 }; // Export both columns
            options.DataTable = dt;

            // Exporter les données vers DataTable
            cells.ExportDataTable(0, 0, 3, 2, options);

            // Affichez les données exportées
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dt.Rows)
            {
                Console.WriteLine($"{row["NumericData"]}, {row["TextData"]}");
            }
        }
    }
}
```

### Voir aussi

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


