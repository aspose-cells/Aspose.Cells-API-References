---
title: "DataLabels.IsTextWrapped"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataLabels-Eigenschaft. Gibt einen Wert zurück oder legt ihn fest, der angibt, ob der Text umgebrochen wird"
type: docs
url: /de/net/aspose.cells.charts/datalabels/istextwrapped/
---
## DataLabels.IsTextWrapped property

Liest oder legt einen Wert fest, der angibt, ob der Text umgebrochen wird.

```csharp
public override bool IsTextWrapped { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyIsTextWrappedDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(85);
            worksheet.Cells["B4"].PutValue(65);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Zugriff auf Datenbeschriftungen
            Aspose.Cells.Charts.DataLabels labels = chart.NSeries[0].DataLabels;
            
            // Datenbeschriftungen anzeigen
            labels.ShowValue = true;
            
            // Demonstration der IsTextWrapped-Eigenschaft
            Console.WriteLine("Before setting IsTextWrapped: " + labels.IsTextWrapped);
            labels.IsTextWrapped = true;
            Console.WriteLine("After setting IsTextWrapped: " + labels.IsTextWrapped);

            // Speichere die Arbeitsmappe
            workbook.Save("DataLabels_IsTextWrapped_Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


