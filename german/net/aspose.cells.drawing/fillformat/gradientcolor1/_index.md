---
title: "FillFormat.GradientColor1"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FillFormat-Eigenschaft. Gibt die Farbverlauffarbe 1 für die angegebene Füllung zurück"
type: docs
url: /de/net/aspose.cells.drawing/fillformat/gradientcolor1/
---
## FillFormat.GradientColor1 property

Gibt die Farbverlauffarbe 1 für die angegebene Füllung zurück.

```csharp
public Color GradientColor1 { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientColor1Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Füllformat der ersten Serie abrufen
            FillFormat fillFormat = chart.NSeries[0].Area.FillFormat;
            
            // Verlaufsfüllung mit korrekten Parametertypen erstellen
            fillFormat.SetTwoColorGradient(
                Color.Red, 
                Color.White, 
                GradientStyleType.Horizontal, 
                1); // Gradient variant must be integer (1-4)

            // Verlaufsfarbe abrufen und anzeigen
            Color gradientColor1 = fillFormat.GradientColor1;
            Console.WriteLine("Gradient Color 1: " + gradientColor1);
            Console.WriteLine("Gradient Degree: " + fillFormat.GradientDegree);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


