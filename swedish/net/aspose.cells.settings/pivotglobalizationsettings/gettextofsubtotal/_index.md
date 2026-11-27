---
title: "PivotGlobalizationSettings.GetTextOfSubTotal"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotGlobalizationSettings‑metoden. Hämtar texten för typen PivotFieldSubtotalType i PivotTable"
type: docs
url: /sv/net/aspose.cells.settings/pivotglobalizationsettings/gettextofsubtotal/
---
## PivotGlobalizationSettings.GetTextOfSubTotal method

Hämtar texten för typen [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) i pivottabellen.

```csharp
public virtual string GetTextOfSubTotal(PivotFieldSubtotalType subTotalType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| subTotalType | PivotFieldSubtotalType | The [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) |

### Returvärde

Texten för given typ

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfSubTotalWithPivotFieldSubtotalTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 1);

            // Skapa globaliseringsinställningar
            Aspose.Cells.Settings.PivotGlobalizationSettings globalizationSettings = new Aspose.Cells.Settings.PivotGlobalizationSettings();

            // Demonstrera GetTextOfSubTotal med olika delsummeringstyper
            Console.WriteLine("Sum Subtotal: " + globalizationSettings.GetTextOfSubTotal(Aspose.Cells.Pivot.PivotFieldSubtotalType.Sum));
            Console.WriteLine("Count Subtotal: " + globalizationSettings.GetTextOfSubTotal(Aspose.Cells.Pivot.PivotFieldSubtotalType.Count));
            Console.WriteLine("Average Subtotal: " + globalizationSettings.GetTextOfSubTotal(Aspose.Cells.Pivot.PivotFieldSubtotalType.Average));
            Console.WriteLine("Max Subtotal: " + globalizationSettings.GetTextOfSubTotal(Aspose.Cells.Pivot.PivotFieldSubtotalType.Max));
            Console.WriteLine("Min Subtotal: " + globalizationSettings.GetTextOfSubTotal(Aspose.Cells.Pivot.PivotFieldSubtotalType.Min));

            // Spara arbetsbok
            workbook.Save("PivotGlobalizationDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PivotFieldSubtotalType](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)
* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


