---
title: "SubtotalSetting.SubtotalFunction"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SubtotalSetting-Eigenschaft. Die Zwischensummenfunktion"
type: docs
url: /de/net/aspose.cells/subtotalsetting/subtotalfunction/
---
## SubtotalSetting.SubtotalFunction property

Die Zwischensummen‑Funktion.

```csharp
public ConsolidationFunction SubtotalFunction { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SubtotalSettingPropertySubtotalFunctionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i % 2 == 0 ? "Group A" : "Group B");
                worksheet.Cells["B" + i].PutValue(i * 100);
            }

            // Erstelle die Zwischensummeinstellung, indem du sie aus vorhandenen Daten abrufst
            CellArea area = CellArea.CreateCellArea("A1", "B10");
            SubtotalSetting subtotalSetting = worksheet.Cells.RetrieveSubtotalSetting(area);
            
            // Konfiguriere Zwischensumme – diese Eigenschaften sind in der tatsächlichen API schreibgeschützt
            // Also werden wir die Subtotal-Methode direkt mit Parametern verwenden
            int groupBy = 0; // Group by first column
            ConsolidationFunction function = ConsolidationFunction.Sum;
            int[] subtotalColumns = new int[] {1}; // Subtotal on second column
            
            // Zwischensummen anwenden
            worksheet.Cells.Subtotal(area, groupBy, function, subtotalColumns);

            // Überprüfe die SubtotalFunction-Eigenschaft aus der abgerufenen Einstellung
            Console.WriteLine("Subtotal Function: " + subtotalSetting.SubtotalFunction);
            
            // Speichere die Arbeitsmappe
            workbook.Save("SubtotalDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


