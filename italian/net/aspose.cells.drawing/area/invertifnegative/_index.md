---
title: "Area.InvertIfNegative"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Area. Se la proprietà è true e il valore del punto del grafico è un numero negativo, il Color di primo piano e il Color di sfondo verranno scambiati"
type: docs
url: /it/net/aspose.cells.drawing/area/invertifnegative/
---
## Area.InvertIfNegative property

Se la proprietà è true e il valore del punto del grafico è un numero negativo, il colore di primo piano e il colore di sfondo verranno scambiati.

```csharp
public bool InvertIfNegative { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AreaPropertyInvertIfNegativeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio con valore negativo
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(-100);
            worksheet.Cells["A3"].PutValue(150);
            
            // Aggiungi un grafico a colonne
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi serie di dati e configura le proprietà dell'area
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries[0].Area.InvertIfNegative = true;
            chart.NSeries[0].Area.ForegroundColor = Color.Red;
            chart.NSeries[0].Area.BackgroundColor = Color.Yellow;
            
            workbook.Save("AreaPropertyInvertIfNegativeDemo.xls");
        }
    }
}
```

### Vedi anche

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


