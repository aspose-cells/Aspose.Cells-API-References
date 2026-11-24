---
title: "PivotItemCollection.ChangeitemsOrder"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotItemCollection-Methode. Ändert die Reihenfolge der beiden Elemente direkt"
type: docs
url: /de/net/aspose.cells.pivot/pivotitemcollection/changeitemsorder/
---
## PivotItemCollection.ChangeitemsOrder method

Ändert die Reihenfolge der beiden Elemente direkt.

```csharp
[Obsolete("Use PivotItemCollection.SwapItem() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ChangeitemsOrder(int sourceIndex, int destIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceIndex | Int32 | Der aktuelle Index |
| destIndex | Int32 | Der Zielindex |

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode PivotItemCollection.SwapItem(). Diese Methode wird 12 Monate später, seit Juli 2024, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

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

### Siehe auch

* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


