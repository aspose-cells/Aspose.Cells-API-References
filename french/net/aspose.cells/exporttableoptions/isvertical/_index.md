---
title: "ExportTableOptions.IsVertical"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExportTableOptions. True si une ligne du fichier Workbook représente une ligne du DataTable. False si une colonne du fichier Workbook représente une ligne du DataTable"
type: docs
url: /fr/net/aspose.cells/exporttableoptions/isvertical/
---
## ExportTableOptions.IsVertical property

True si une ligne du fichier Workbook représente une ligne dans le DataTable. False si une colonne du fichier Workbook représente une ligne dans le DataTable.

```csharp
public bool IsVertical { get; set; }
```

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyIsVerticalDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Créer des données d'exemple dans la feuille de calcul
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(25);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(30);

            // Créer un DataTable
            DataTable dt = new DataTable();
            dt.Columns.Add("Column1", typeof(string));
            dt.Columns.Add("Column2", typeof(int));

            // Définir ExportTableOptions avec IsVertical = true
            ExportTableOptions options = new ExportTableOptions();
            options.IsVertical = true;
            options.ExportColumnName = true;
            options.DataTable = dt;

            // Exporter les données verticalement
            cells.ExportDataTable(0, 0, 2, 2, options);

            // Afficher le DataTable exporté
            foreach (DataRow row in dt.Rows)
            {
                Console.WriteLine($"{row[0]}, {row[1]}");
            }
        }
    }
}
```

### Voir aussi

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


