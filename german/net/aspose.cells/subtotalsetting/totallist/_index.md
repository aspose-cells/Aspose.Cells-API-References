---
title: "SubtotalSetting.TotalList"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SubtotalSetting-Eigenschaft. Ein Array von nullbasierten Feldversätzen, die die Felder angeben, zu denen die Zwischensummen hinzugefügt werden"
type: docs
url: /de/net/aspose.cells/subtotalsetting/totallist/
---
## SubtotalSetting.TotalList property

Ein Array von nullbasierten Feld‑Offsets, das die Felder angibt, zu denen die Zwischensummen hinzugefügt werden.

```csharp
public int[] TotalList { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SubtotalSettingPropertyTotalListDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten einrichten
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Zwischensumme erstellen und anwenden
            CellArea area = CellArea.CreateCellArea("A1", "B5");
            worksheet.Cells.Subtotal(area, 0, ConsolidationFunction.Sum, new int[] { 1 }, true, true, true);

            // Rufe die Zwischensummeneinstellung ab, um die Verwendung von TotalList zu demonstrieren
            SubtotalSetting subtotal = worksheet.Cells.RetrieveSubtotalSetting(area);
            Console.WriteLine("TotalList contains column index: " + subtotal.TotalList[0]);
            
            // Speichere die Arbeitsmappe
            workbook.Save("SubtotalDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


