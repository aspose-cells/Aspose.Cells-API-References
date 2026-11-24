---
title: "PivotOptions.DropZoneCategories"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotOptions-Eigenschaft. Gibt an, ob für jedes PivotTable-Feld auf der Zeilenachse der Quell-PivotTable ein Steuerelement im Diagramm angezeigt wird, wenn dropZonesVisible auf true gesetzt ist."
type: docs
url: /de/net/aspose.cells.charts/pivotoptions/dropzonecategories/
---
## PivotOptions.DropZoneCategories property

Gibt an, ob ein Steuerelement für jedes PivotTable‑Feld auf der Zeilenachse der Quell‑PivotTable im Diagramm angezeigt wird, wenn dropZonesVisible auf true gesetzt ist.

```csharp
public bool DropZoneCategories { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZoneCategoriesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Ein Arbeitsblatt und einige Beispieldaten hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            
            // Ein Diagramm hinzufügen, das Pivot-Daten verwendet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Auf Pivot-Optionen aus dem Diagramm zugreifen
            PivotOptions options = chart.PivotOptions;
            
            // DropZoneCategories-Eigenschaft demonstrieren
            options.DropZoneCategories = true;
            Console.WriteLine("DropZoneCategories enabled: " + options.DropZoneCategories);
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotOptionsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


