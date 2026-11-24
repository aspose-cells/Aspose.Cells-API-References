---
title: "SeriesCollection.CategoryData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SeriesCollection Eigenschaft. Gibt den Bereich der Kategorie-Achsenwerte zurück oder setzt ihn. Es kann ein Zellbereich wie d1e10 oder eine Wertefolge wie 26810 sein."
type: docs
url: /de/net/aspose.cells.charts/seriescollection/categorydata/
---
## SeriesCollection.CategoryData property

Liest oder setzt den Bereich der Kategorienachsenwerte. Es kann ein Zellbereich sein (z. B. "d1:e10") oder eine Wertefolge (z. B. "{2,6,8,10}").

```csharp
public string CategoryData { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionPropertyCategoryDataDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue("Cat " + (i - 1));
                worksheet.Cells["B" + i].PutValue(i * 10);
            }
            
            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("=Sheet1!$B$2:$B$10", true);
            chart.NSeries.CategoryData = "=Sheet1!$A$2:$A$10";
            
            // Speichere die Arbeitsmappe
            workbook.Save("CategoryDataDemo.xlsx");
            
            // Überprüfen Sie die CategoryData-Eigenschaft
            Console.WriteLine("Chart CategoryData: " + chart.NSeries.CategoryData);
        }
    }
}
```

### Siehe auch

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


