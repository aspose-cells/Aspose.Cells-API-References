---
title: "Axis.AxisLabels"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà dell'asse. Ottiene le etichette dell'asse dopo la chiamata al metodo Chart.Calculate"
type: docs
url: /it/net/aspose.cells.charts/axis/axislabels/
---
## Axis.AxisLabels property

Ottiene le etichette dell'asse dopo aver chiamato il metodo Chart.Calculate().

```csharp
[Obsolete("Use Axis.GetAxisTexts method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList AxisLabels { get; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo Axis.GetAxisTexts. Questa proprietà sarà rimossa tra 12 mesi a partire da novembre 2023. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisPropertyAxisLabelsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
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

            try
            {
                // Aggiungi un grafico al foglio di lavoro
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
                Chart chart = worksheet.Charts[chartIndex];

                // Imposta l'intervallo dati del grafico
                chart.NSeries.Add("B2:B4", true);
                chart.NSeries.CategoryData = "A2:A4";

                // Calcola il grafico per generare le etichette dell'asse
                chart.Calculate();

                // Accedi all'asse delle categorie e ottieni le etichette dell'asse
                Axis categoryAxis = chart.CategoryAxis;
                var axisLabels = categoryAxis.AxisLabels;

                // Visualizza le etichette dell'asse
                Console.WriteLine("Axis Labels:");
                if (axisLabels != null)
                {
                    foreach (var label in axisLabels)
                    {
                        Console.WriteLine(label);
                    }
                }
                else
                {
                    Console.WriteLine("No axis labels available.");
                }

                // Salva la cartella di lavoro
                workbook.Save("AxisPropertyAxisLabelsDemo.xlsx");
                Console.WriteLine("AxisLabels demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


