---
title: "Axis.MajorTickMark"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Axis. Rappresenta il tipo di segno di graduazione principale per l'asse specificato"
type: docs
url: /it/net/aspose.cells.charts/axis/majortickmark/
---
## Axis.MajorTickMark property

Rappresenta il tipo di segnapunto principale per l'asse specificato.

```csharp
public TickMarkType MajorTickMark { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMajorTickMarkDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico a colonne
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Imposta il tipo di segno di graduazione principale su esterno
            chart.ValueAxis.MajorTickMark = TickMarkType.Outside;

            // Salva la cartella di lavoro
            workbook.Save("AxisPropertyMajorTickMarkDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TickMarkType](../../tickmarktype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


