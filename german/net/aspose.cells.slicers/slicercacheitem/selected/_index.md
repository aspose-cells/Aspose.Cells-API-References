---
title: "SlicerCacheItem.Selected"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SlicerCacheItem-Eigenschaft. Gibt an, ob das SlicerCacheItem ausgewählt ist oder nicht"
type: docs
url: /de/net/aspose.cells.slicers/slicercacheitem/selected/
---
## SlicerCacheItem.Selected property

Gibt an, ob das [`SlicerCacheItem`](../) ausgewählt ist oder nicht.

```csharp
public bool Selected { get; set; }
```

### Hinweise

Verwenden Sie stattdessen die Methode [`SelectItems`](../../slicer/selectitems/), wenn Sie ein Element auswählen möchten. Da dieser Aktualisierungsvorgang bei jeder Auswahländerung eine vollständige Datenneuladung verursacht, führt er zu schlechter Leistung.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCacheItemPropertySelectedDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten für Pivot‑Tabelle erstellen
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Pivot-Tabelle erstellen
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Füge Slicer hinzu
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "Slicer1");
            Aspose.Cells.Slicers.Slicer slicer = worksheet.Slicers[slicerIndex];
            slicer.StyleType = SlicerStyleType.SlicerStyleLight1;

            // Auf Slicer-Cache-Elemente zugreifen
            for (int i = 0; i < slicer.SlicerCache.SlicerCacheItems.Count; i++)
            {
                SlicerCacheItem item = slicer.SlicerCache.SlicerCacheItems[i];
                
                // Erstes Element auswählen, andere abwählen
                if (i == 0)
                {
                    item.Selected = true;
                    Console.WriteLine($"Item '{item.Value}' is selected: {item.Selected}");
                }
                else
                {
                    item.Selected = false;
                    Console.WriteLine($"Item '{item.Value}' is selected: {item.Selected}");
                }
            }

            // Speichere die Arbeitsmappe
            workbook.Save("SlicerCacheItemSelectedDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SlicerCacheItem](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


