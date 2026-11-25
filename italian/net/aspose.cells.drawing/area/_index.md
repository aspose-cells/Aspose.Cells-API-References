---
title: "Classe Area"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.Area class. Incapsula l'oggetto che rappresenta un formato area"
type: docs
url: /it/net/aspose.cells.drawing/area/
---
## Area class

Incapsula l'oggetto che rappresenta un formato area.

```csharp
public class Area
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor/) { get; set; } | Ottiene o imposta il colore di sfondo dell'`Area`. |
| [FillFormat](../../aspose.cells.drawing/area/fillformat/) { get; } | Rappresenta un oggetto [`FillFormat`](./fillformat/) che contiene le proprietà di formattazione del riempimento per il grafico o la forma specificati. |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor/) { get; set; } | Ottiene o imposta il colore di primo piano. |
| [Formatting](../../aspose.cells.drawing/area/formatting/) { get; set; } | Rappresenta la formattazione dell'area. |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative/) { get; set; } | Se la proprietà è true e il valore del punto del grafico è un numero negativo, il colore di primo piano e il colore di sfondo verranno scambiati. |
| [Transparency](../../aspose.cells.drawing/area/transparency/) { get; set; } | Restituisce o imposta il grado di trasparenza dell'area come valore da 0,0 (opaco) a 1,0 (trasparente). |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class AreaDemo
    {
        public static void AreaExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();
            // Aggiungere un nuovo foglio di lavoro all'oggetto Workbook
            int sheetIndex = workbook.Worksheets.Add();
            // Ottenere il riferimento del foglio di lavoro appena aggiunto passando il suo indice di foglio
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Aggiunta di valori di esempio alle celle
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(-100);
            worksheet.Cells["A3"].PutValue(150);
            // Aggiunta di un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 15, 5);
            // Accesso all'istanza del grafico appena aggiunto
            Chart chart = worksheet.Charts[chartIndex];
            // Aggiunta di NSeries (origine dati del grafico) al grafico dall'intervallo di celle "A1" a "A3"
            chart.NSeries.Add("A1:A3", true);

            // Accesso all'area del primo NSeries
            Area area = chart.NSeries[0].Area;

            // Impostazione delle proprietà
            area.InvertIfNegative = true;
            area.ForegroundColor = Color.Red;
            area.BackgroundColor = Color.Yellow;
            area.Formatting = Aspose.Cells.Charts.FormattingType.Custom;
            area.Transparency = 0.5;

            // Salvataggio del file Excel
            workbook.Save("AreaExample.xlsx");
            workbook.Save("AreaExample.pdf");

        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


