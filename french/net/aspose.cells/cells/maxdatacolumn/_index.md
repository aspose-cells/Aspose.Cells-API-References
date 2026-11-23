---
title: "Cells.MaxDataColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells. Index de colonne maximal de la cellule contenant des données"
type: docs
url: /fr/net/aspose.cells/cells/maxdatacolumn/
---
## Cells.MaxDataColumn property

Indice de colonne maximal de la cellule contenant des données.

```csharp
public int MaxDataColumn { get; }
```

### Remarques

-1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet dynamically, so it is a time-consumed progress and should not be invoked repeatedly, such as using it directly as condition in a loop.

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Data;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxDataColumnDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(300);
            worksheet.Cells["B3"].PutValue(400);

            // Obtenez l'index de colonne de données maximal (base 0)
            int maxColumn = worksheet.Cells.MaxDataColumn;
            Console.WriteLine("Max Data Column: " + maxColumn);

            // Exportez les données en utilisant MaxDataColumn
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 
                worksheet.Cells.MaxDataRow + 1, 
                worksheet.Cells.MaxDataColumn + 1);

            // Affichez les données exportées
            Console.WriteLine("Exported Data:");
            foreach (DataRow row in dataTable.Rows)
            {
                for (int i = 0; i <= maxColumn; i++)
                {
                    Console.Write(row[i] + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


