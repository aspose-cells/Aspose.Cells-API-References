---
title: "PivotItemCollection.ChangeitemsOrder"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotItemCollection. Change directement l'ordre des deux éléments"
type: docs
url: /fr/net/aspose.cells.pivot/pivotitemcollection/changeitemsorder/
---
## PivotItemCollection.ChangeitemsOrder method

Change directement l'ordre des deux éléments.

```csharp
[Obsolete("Use PivotItemCollection.SwapItem() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ChangeitemsOrder(int sourceIndex, int destIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceIndex | Int32 | L'index actuel |
| destIndex | Int32 | L'index de destination |

### Remarques

REMARQUE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode PivotItemCollection.SwapItem(). Cette méthode sera supprimée 12 mois plus tard à compter de juillet 2024. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemCollectionMethodChangeitemsOrderWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells[0, 0].Value = "Category";
            worksheet.Cells[1, 0].Value = "A";
            worksheet.Cells[2, 0].Value = "B";
            worksheet.Cells[3, 0].Value = "C";

            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:A4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            Console.WriteLine("Original Order:");
            foreach (PivotItem item in pivotItems)
            {
                Console.WriteLine(item.Name);
            }

            pivotItems.ChangeitemsOrder(0, 2);

            Console.WriteLine("\nAfter Changing Order:");
            foreach (PivotItem item in pivotItems)
            {
                Console.WriteLine(item.Name);
            }

            workbook.Save("PivotItemOrderChange.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


