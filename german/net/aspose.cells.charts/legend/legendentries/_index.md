---
title: "Legend.LegendEntries"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Legend-Eigenschaft. Gibt eine Sammlung aller LegendEntry-Objekte in der angegebenen Diagrammlegende zurück. Das Festlegen der Legendeinträge des Oberflächendiagramms wird nicht unterstützt. Daher wird null zurückgegeben, wenn der Diagrammtyp ein Oberflächendiagramm ist."
type: docs
url: /de/net/aspose.cells.charts/legend/legendentries/
---
## Legend.LegendEntries property

Liest eine Sammlung aller LegendEntry-Objekte in der angegebenen Diagrammlegende. Das Festlegen der Legendeinträge des Oberflächendiagramms wird nicht unterstützt. Daher wird null zurückgegeben, wenn der Diagrammtyp ein Oberflächendiagramm ist.

```csharp
public LegendEntryCollection LegendEntries { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendPropertyLegendEntriesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.CategoryData = "B2:B4";

            // Zugriff auf Legendeinträge
            Aspose.Cells.Charts.LegendEntryCollection legendEntries = chart.Legend.LegendEntries;
            
            // Lösche den zweiten Legendeneintrag
            legendEntries[1].IsDeleted = true;
            
            // Speichere die Arbeitsmappe
            workbook.Save("LegendEntriesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [LegendEntryCollection](../../legendentrycollection/)
* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


