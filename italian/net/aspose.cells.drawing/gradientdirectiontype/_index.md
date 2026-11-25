---
title: "Enum GradientDirectionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.GradientDirectionType enum. Rappresenta tutti i tipi di direzione del gradiente"
type: docs
url: /it/net/aspose.cells.drawing/gradientdirectiontype/
---
## GradientDirectionType enumeration

Rappresenta tutti i tipi di direzione del gradiente.

```csharp
public enum GradientDirectionType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| FromUpperLeftCorner | `0` | FromUpperLeftCorner |
| FromUpperRightCorner | `1` | FromUpperRightCorner |
| FromLowerLeftCorner | `2` | FromLowerLeftCorner |
| FromLowerRightCorner | `3` | FromLowerRightCorner |
| FromCenter | `4` | FromCenter |
| Unknown | `5` | Sconosciuto |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientDirectionTypeDemo
    {
        public static void GradientDirectionTypeExample()
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

            // Accedi all'area del tracciato del grafico
            PlotArea plotArea = chart.PlotArea;

            // Accedi al formato di riempimento dell'area del tracciato
            FillFormat fillFormat = plotArea.Area.FillFormat;

            // Imposta un riempimento a gradiente bicolore con una direzione specifica
            fillFormat.SetTwoColorGradient(Color.Blue, Color.LightBlue, GradientStyleType.DiagonalDown, 1);
            fillFormat.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromUpperLeftCorner);

            // Restituisci il tipo di direzione del gradiente
            Console.WriteLine("Gradient Direction Type: " + fillFormat.GradientFill.DirectionType);

            // Salva la cartella di lavoro
            workbook.Save("GradientDirectionTypeExample.xlsx");
            workbook.Save("GradientDirectionTypeExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


