---
title: "Axis.DisplayUnitLabel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Axis. Rappresenta un'etichetta di unità su un asse nel grafico specificato. Le etichette di unità sono utili per rappresentare valori grandi, ad esempio in milioni o miliardi"
type: docs
url: /it/net/aspose.cells.charts/axis/displayunitlabel/
---
## Axis.DisplayUnitLabel property

Rappresenta un'etichetta dell'unità su un asse nel grafico specificato. Le etichette delle unità sono utili per rappresentare valori grandi, ad esempio in milioni o miliardi.

```csharp
public DisplayUnitLabel DisplayUnitLabel { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyDisplayUnitLabelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(1000);
            worksheet.Cells["A2"].PutValue(2000);
            worksheet.Cells["A3"].PutValue(3000);
            worksheet.Cells["A4"].PutValue(4000);
            
            // Crea grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("A1:A4", true);
            
            // Configura unità di visualizzazione ed etichetta
            chart.ValueAxis.DisplayUnit = Aspose.Cells.Charts.DisplayUnitType.Thousands;
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            // Genera il testo dell'etichetta dell'unità di visualizzazione
            Console.WriteLine("Display Unit Label: " + chart.ValueAxis.DisplayUnitLabel.Text);
            
            // Salva la cartella di lavoro
            workbook.Save("AxisPropertyDisplayUnitLabelDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [DisplayUnitLabel](../../displayunitlabel/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


