---
title: "FillFormat.GradientDegree"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FillFormat. Restituisce il grado del gradiente per il riempimento specificato. Valido solo per Excel 2007"
type: docs
url: /it/net/aspose.cells.drawing/fillformat/gradientdegree/
---
## FillFormat.GradientDegree property

Restituisce il grado del gradiente per il riempimento specificato. Valido solo per Excel 2007.

```csharp
public double GradientDegree { get; }
```

### Osservazioni

Può essere solo un valore da 0.0 (scuro) a 1.0 (chiaro).

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientDegreeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Imposta il riempimento gradiente per la prima serie
            Aspose.Cells.Drawing.FillFormat fillFormat = chart.NSeries[0].Area.FillFormat;
            fillFormat.SetTwoColorGradient(Color.Red, Color.Blue, Aspose.Cells.Drawing.GradientStyleType.Horizontal, 2);
            
            // Visualizza il grado del gradiente
            Console.WriteLine("Gradient Degree: " + fillFormat.GradientDegree);

            // Salva la cartella di lavoro
            workbook.Save("GradientDegreeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


