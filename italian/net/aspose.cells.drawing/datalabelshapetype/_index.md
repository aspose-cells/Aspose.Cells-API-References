---
title: "Enum DataLabelShapeType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.DataLabelShapeType enum. Specifica la geometria della forma predefinita da utilizzare per un grafico"
type: docs
url: /it/net/aspose.cells.drawing/datalabelshapetype/
---
## DataLabelShapeType enumeration

Specifica la geometria della forma predefinita da utilizzare per un grafico.

```csharp
public enum DataLabelShapeType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Rect | `0` | Rappresenta la forma rettangolare. |
| RoundRect | `1` | Rappresenta la forma del rettangolo arrotondato. |
| Ellipse | `2` | Rappresenta la forma dell'ellisse. |
| RightArrowCallout | `3` | Rappresenta la forma della callout a freccia destra. |
| DownArrowCallout | `4` | Rappresenta la forma della callout a freccia verso il basso. |
| LeftArrowCallout | `5` | Rappresenta la forma della callout a freccia sinistra. |
| UpArrowCallout | `6` | Rappresenta la forma della callout a freccia verso l'alto. |
| WedgeRectCallout | `7` | Rappresenta la forma della callout a cuneo rettangolare. |
| WedgeRoundRectCallout | `8` | Rappresenta la forma della callout a cuneo rettangolo arrotondato. |
| WedgeEllipseCallout | `9` | Rappresenta la forma della callout a cuneo ellittico. |
| LineCallout | `10` | Rappresenta la forma della callout a linea. |
| BentLineCallout | `11` | Rappresenta la forma della callout a linea piegata. |
| LineWithAccentBarCallout | `12` | Rappresenta la forma della callout a linea con barra di accento. |
| BentLineWithAccentBarCallout | `13` | Rappresenta la forma della callout a linea piegata con barra di accento. |
| Line | `14` | Questo tipo è utilizzato solo per l'elaborazione speciale di file. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class DataLabelShapeTypeDemo
    {
        public static void DataLabelShapeTypeExample()
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

            // Accedi alla prima serie nel grafico
            Series series = chart.NSeries[0];

            // Abilita le etichette dati per la serie.
            series.DataLabels.ShowValue = true;
            series.DataLabels.ShapeType = DataLabelShapeType.RoundRect;

            // Salva la cartella di lavoro
            workbook.Save("DataLabelShapeTypeExample.xlsx");
            workbook.Save("DataLabelShapeTypeExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


