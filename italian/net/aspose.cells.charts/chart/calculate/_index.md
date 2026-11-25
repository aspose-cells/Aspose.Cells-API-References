---
title: "Chart.Calculate"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Chart. Calcola le posizioni personalizzate dell'area del grafico e degli assi se le loro posizioni sono assegnate automaticamente"
type: docs
url: /it/net/aspose.cells.charts/chart/calculate/
---
## Calculate() {#calculate}

Calcola le posizioni personalizzate dell'area del grafico e degli assi se le loro posizioni sono assegnate automaticamente.

```csharp
public void Calculate()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodCalculateDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcola il grafico prima di salvare
            chart.Calculate();

            // Salva la cartella di lavoro con il grafico
            workbook.Save("ChartCalculateDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Calculate(ChartCalculateOptions) {#calculate_1}

Calcola la posizione personalizzata dell'area del grafico e degli assi se le loro posizioni sono assegnate automaticamente, con le Opzioni di Calcolo del Grafico.

```csharp
public void Calculate(ChartCalculateOptions calculateOptions)
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodCalculateWithChartCalculateOptionsDemo
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
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(150);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Abilita le etichette dei dati
            chart.NSeries[0].DataLabels.ShowValue = true;

            // Crea le opzioni di calcolo e impostale per aggiornare tutti i punti
            ChartCalculateOptions calculateOptions = new ChartCalculateOptions();
            calculateOptions.UpdateAllPoints = true;

            // Calcola il grafico con opzioni
            chart.Calculate(calculateOptions);

            // Genera i testi delle etichette dei dati
            ChartPointCollection points = chart.NSeries[0].Points;
            Console.WriteLine("DataLabel Text for Point 0: " + points[0].DataLabels.Text);
            Console.WriteLine("DataLabel Text for Point 1: " + points[1].DataLabels.Text);
            Console.WriteLine("DataLabel Text for Point 2: " + points[2].DataLabels.Text);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartCalculateOptions](../../chartcalculateoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


