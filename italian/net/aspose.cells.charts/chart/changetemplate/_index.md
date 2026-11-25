---
title: "Chart.ChangeTemplate"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Chart. Cambia il tipo di grafico con un modello predefinito"
type: docs
url: /it/net/aspose.cells.charts/chart/changetemplate/
---
## Chart.ChangeTemplate method

Cambia il tipo di grafico con un modello predefinito.

```csharp
public void ChangeTemplate(byte[] data)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dati | Byte[] | I dati del file modello del grafico (.crtx). |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.IO;

    public class ChartMethodChangeTemplateWithByteDemo
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

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.SetChartDataRange("A1:B4", false);

            // Ottieni i dati del modello da un altro file di grafico
            byte[] templateData = File.ReadAllBytes("ChartTemplate.crtx");

            try
            {
                // Chiama il metodo ChangeTemplate con parametro array di byte
                chart.ChangeTemplate(templateData);
                
                Console.WriteLine("Chart template changed successfully using byte array parameter");
                
                // Mostra l'effetto salvando la cartella di lavoro
                workbook.Save("ChartWithChangedTemplate.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error changing chart template: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


