---
title: "TrendlineCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo TrendlineCollection. Aggiunge un oggetto Trendline a questa collezione con il tipo specificato"
type: docs
url: /it/net/aspose.cells.charts/trendlinecollection/add/
---
## Add(TrendlineType) {#add}

Aggiunge un oggetto [`Trendline`](../../trendline/) a questa collezione con il tipo specificato.

```csharp
public int Add(TrendlineType type)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | TrendlineType | Tipo di Trendline. |

### Valore di ritorno

[`Trendline`](../../trendline/) object index.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlineCollectionMethodAddWithTrendlineTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["B3"].PutValue(4);
            worksheet.Cells["B4"].PutValue(8);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi dati della serie
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Aggiungi una trendline esponenziale alla prima serie
            chart.NSeries[0].TrendLines.Add(TrendlineType.Exponential);

            // Salva la cartella di lavoro
            workbook.Save("TrendlineCollectionMethodAddWithTrendlineTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TrendlineType](../../trendlinetype/)
* class [TrendlineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(TrendlineType, string) {#add_1}

Aggiunge un oggetto [`Trendline`](../../trendline/) a questa collezione con tipo e nome specificati.

```csharp
public int Add(TrendlineType type, string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | TrendlineType | Tipo di Trendline. |
| name | String | Nome della Trendline. |

### Valore di ritorno

[`Trendline`](../../trendline/) object index.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlineCollectionMethodAddWithTrendlineTypeStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("X Values");
            sheet.Cells["B1"].PutValue("Y Values");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue(i);
                sheet.Cells["B" + i].PutValue(i * 2);
            }

            // Crea grafico
            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Aggiungi serie e imposta i dati
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries[0].XValues = "A2:A10";
            chart.NSeries[0].Name = "Data Series";

            // Aggiungi trendline con TrendlineType e nome
            chart.NSeries[0].TrendLines.Add(TrendlineType.Logarithmic, "Logarithmic Trend");
            
            // Imposta alcune proprietà della trendline
            Trendline trendline = chart.NSeries[0].TrendLines[0];
            trendline.DisplayEquation = true;
            trendline.DisplayRSquared = true;
            
            workbook.Save("TrendlineDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TrendlineType](../../trendlinetype/)
* class [TrendlineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


