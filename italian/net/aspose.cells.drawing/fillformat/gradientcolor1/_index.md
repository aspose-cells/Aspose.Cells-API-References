---
title: "FillFormat.GradientColor1"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FillFormat. Restituisce il colore gradiente 1 per il riempimento specificato"
type: docs
url: /it/net/aspose.cells.drawing/fillformat/gradientcolor1/
---
## FillFormat.GradientColor1 property

Restituisce il colore gradiente 1 per il riempimento specificato.

```csharp
public Color GradientColor1 { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Ottieni il formato di riempimento della prima serie
            FillFormat fillFormat = chart.NSeries[0].Area.FillFormat;
            
            // Crea un riempimento gradiente usando i tipi di parametro corretti
            fillFormat.SetTwoColorGradient(
                Color.Red, 
                Color.White, 
                GradientStyleType.Horizontal, 
                1); // Gradient variant must be integer (1-4)

            // Ottieni e visualizza il colore gradiente
            Color gradientColor1 = fillFormat.GradientColor1;
            Console.WriteLine("Gradient Color 1: " + gradientColor1);
            Console.WriteLine("Gradient Degree: " + fillFormat.GradientDegree);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


