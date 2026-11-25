---
title: "Enum MsoLineStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.MsoLineStyle enum. Rappresenta lo stile delle linee di disegno"
type: docs
url: /it/net/aspose.cells.drawing/msolinestyle/
---
## MsoLineStyle enumeration

Rappresenta lo stile delle linee di disegno.

```csharp
public enum MsoLineStyle
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Single | `0` | Linea singola (di larghezza lineWidth) |
| ThickBetweenThin | `1` | Tre linee, sottile, spessa, sottile |
| ThinThick | `2` | Linee doppie, una sottile, una spessa |
| ThickThin | `3` | Linee doppie, una spessa, una sottile |
| ThinThin | `4` | Linee doppie di larghezza uguale |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineStyleDemo
    {
        public static void MsoLineStyleExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.SetChartDataRange("A1:B4", true);

            // Accedi all'asse di categoria primario
            Axis categoryAxis = chart.CategoryAxis;

            // Imposta lo stile della linea per l'asse di categoria primario
            Line axisLine = categoryAxis.AxisLine;
            axisLine.CompoundType = MsoLineStyle.ThickBetweenThin;
            axisLine.Color = Color.Blue;
            axisLine.WeightPt = 2.0;

            // Restituisci lo stile della linea
            Console.WriteLine("Axis Line Style: " + axisLine.CompoundType);
            Console.WriteLine("Axis Line Color: " + axisLine.Color);
            Console.WriteLine("Axis Line Weight: " + axisLine.WeightPt);

            // Salva la cartella di lavoro
            workbook.Save("MsoLineStyleExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


