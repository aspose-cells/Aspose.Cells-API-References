---
title: "SubtotalSetting.SummaryBelowData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SubtotalSetting‑Eigenschaft. Gibt an, ob eine Zusammenfassung unter den Daten hinzugefügt wird"
type: docs
url: /de/net/aspose.cells/subtotalsetting/summarybelowdata/
---
## SubtotalSetting.SummaryBelowData property

Gibt an, ob eine Zusammenfassung unter den Daten hinzugefügt wird.

```csharp
public bool SummaryBelowData { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SubtotalSettingPropertySummaryBelowDataDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["A4"].PutValue("B");
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Erstellen Sie einen Zellenbereich für Zwischensummen
            CellArea area = CellArea.CreateCellArea("A1", "B5");

            // Wenden Sie Zwischensummen mit der Cells.Subtotal‑Methode und allen erforderlichen Parametern an
            worksheet.Cells.Subtotal(
                area, 
                0, 
                ConsolidationFunction.Sum, 
                new int[] { 1 }, 
                false, 
                false, 
                false);  // summaryBelowData parameter

            // Rufen Sie die Einstellung ab, um SummaryBelowData zu prüfen
            SubtotalSetting retrievedSetting = worksheet.Cells.RetrieveSubtotalSetting(area);
            
            // Geben Sie den Wert der SummaryBelowData‑Eigenschaft aus
            Console.WriteLine("SummaryBelowData: " + retrievedSetting.SummaryBelowData);
        }
    }
}
```

### Siehe auch

* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


