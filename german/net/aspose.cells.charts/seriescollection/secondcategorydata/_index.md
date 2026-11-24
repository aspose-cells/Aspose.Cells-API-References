---
title: "SeriesCollection.SecondCategoryData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SeriesCollection Eigenschaft. Gibt den Bereich der zweiten Kategorie-Achsenwerte zurück oder setzt ihn. Es kann ein Zellbereich wie d1e10 oder eine Wertefolge wie 26810 sein. Wirkt nur, wenn einige Serien auf der zweiten Achse dargestellt wurden."
type: docs
url: /de/net/aspose.cells.charts/seriescollection/secondcategorydata/
---
## SeriesCollection.SecondCategoryData property

Liest oder setzt den Bereich der zweiten Kategorienachsenwerte. Es kann ein Zellbereich sein (z. B. "d1:e10") oder eine Wertefolge (z. B. "{2,6,8,10}"). Wirkt nur, wenn einige Serien auf der zweiten Achse dargestellt wurden.

```csharp
public string SecondCategoryData { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionPropertySecondCategoryDataDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Primary Categories");
            worksheet.Cells["A2"].PutValue("Cat1");
            worksheet.Cells["A3"].PutValue("Cat2");
            worksheet.Cells["A4"].PutValue("Cat3");
            
            worksheet.Cells["B1"].PutValue("Secondary Categories");
            worksheet.Cells["B2"].PutValue("SubCat1");
            worksheet.Cells["B3"].PutValue("SubCat2");
            worksheet.Cells["B4"].PutValue("SubCat3");
            
            worksheet.Cells["C1"].PutValue("Values");
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(20);
            worksheet.Cells["C4"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Seriendaten festlegen
            chart.NSeries.Add("C2:C4", true);
            
            // Primäre Kategoriedaten festlegen
            chart.NSeries.CategoryData = "A2:A4";
            
            // Sekundäre Kategoriedaten festlegen
            chart.NSeries.SecondCategoryData = "B2:B4";

            // Speichere die Arbeitsmappe
            workbook.Save("SecondCategoryDataDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


