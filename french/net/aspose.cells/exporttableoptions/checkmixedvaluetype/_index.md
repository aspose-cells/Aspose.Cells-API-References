---
title: "ExportTableOptions.CheckMixedValueType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExportTableOptions. False Aspose.Cells définira le type de DataColumns selon le type de valeur de la première ligne pour des performances optimales. True Aspose.Cells vérifiera si le type de valeur dans la colonne est mixte avant de définir le type de DataColumns. Et si le type de valeur est mixte, le type de DataColumns sera string."
type: docs
url: /fr/net/aspose.cells/exporttableoptions/checkmixedvaluetype/
---
## ExportTableOptions.CheckMixedValueType property

False, Aspose.Cells définira le type du DataColumn en fonction du type de valeur de la première ligne pour des raisons de performance. True, Aspose.Cells vérifiera si le type de valeur dans la colonne est mixte avant de définir le type du DataColumn. Si les types de valeur sont mixtes, le type du DataColumn sera string.

```csharp
public bool CheckMixedValueType { get; set; }
```

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyCheckMixedValueTypeDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des en-têtes
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value Date");

            // Ajouter des données d'exemple avec des types mixtes
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(DateTime.Now);
            worksheet.Cells["A3"].PutValue(2.5);
            worksheet.Cells["B3"].PutValue("2023-01-15");
            worksheet.Cells["A4"].PutValue("3");
            worksheet.Cells["B4"].PutValue(DateTime.Now.AddDays(1));

            // Créer des options d'exportation avec CheckMixedValueType activé
            ExportTableOptions options = new ExportTableOptions
            {
                CheckMixedValueType = true,
                ExportColumnName = true
            };

            // Exporter les données vers DataTable
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 4, 2, options);

            // Afficher les résultats
            Console.WriteLine("Columns: " + dataTable.Columns.Count);
            Console.WriteLine("Rows: " + dataTable.Rows.Count);
            Console.WriteLine("ID column type: " + dataTable.Columns["ID"].DataType);
            Console.WriteLine("Value Date column type: " + dataTable.Columns["Value Date"].DataType);
        }
    }
}
```

### Voir aussi

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


