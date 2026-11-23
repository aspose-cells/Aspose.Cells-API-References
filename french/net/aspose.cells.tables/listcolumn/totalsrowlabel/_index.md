---
title: "ListColumn.TotalsRowLabel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListColumn. Obtient et définit les libellés d'affichage de la ligne de total"
type: docs
url: /fr/net/aspose.cells.tables/listcolumn/totalsrowlabel/
---
## ListColumn.TotalsRowLabel property

Obtient et définit les libellés d’affichage de la ligne de total.

```csharp
public string TotalsRowLabel { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyTotalsRowLabelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["A4"].PutValue("Item3");
            worksheet.Cells["B4"].PutValue(200);

            // Créez un tableau
            int index = worksheet.ListObjects.Add(0, 0, 4, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.ShowTotals = true;

            // Configurer la ligne de total
            ListColumn priceColumn = table.ListColumns[1];
            priceColumn.TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;
            priceColumn.TotalsRowLabel = "Grand Total";

            workbook.Save("ListColumnTotalsRowLabelDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


