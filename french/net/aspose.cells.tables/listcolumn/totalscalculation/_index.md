---
title: "ListColumn.TotalsCalculation"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListColumn. Obtient et définit le type de calcul dans la ligne Totals du ListColumn"
type: docs
url: /fr/net/aspose.cells.tables/listcolumn/totalscalculation/
---
## ListColumn.TotalsCalculation property

Obtient et définit le type de calcul dans la ligne Totaux de la colonne de liste.

```csharp
public TotalsCalculation TotalsCalculation { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyTotalsCalculationDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["A4"].PutValue("Item 3");
            worksheet.Cells["B4"].PutValue(200);

            // Créer un objet de liste
            int listObjIndex = worksheet.ListObjects.Add(0, 0, 4, 1, true);
            ListObject listObj = worksheet.ListObjects[listObjIndex];
            listObj.ShowTotals = true;
            
            // Définissez le calcul des totaux pour la deuxième colonne
            listObj.ListColumns[1].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // Enregistrez le classeur
            workbook.Save("ListColumnTotalsCalculationDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TotalsCalculation](../../totalscalculation/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


