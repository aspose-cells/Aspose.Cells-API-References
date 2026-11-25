---
title: "Area.Transparency"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Area. Restituisce o imposta il grado di trasparenza dell'area come valore da 0.0 opaco a 1.0 trasparente"
type: docs
url: /it/net/aspose.cells.drawing/area/transparency/
---
## Area.Transparency property

Restituisce o imposta il grado di trasparenza dell'area come valore da 0,0 (opaco) a 1,0 (trasparente).

```csharp
public double Transparency { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AreaPropertyTransparencyDemo
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

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accedi alla prima serie
            Aspose.Cells.Charts.Series series = chart.NSeries[0];

            // Dimostra la proprietà Transparency
            Console.WriteLine("Initial area transparency: " + series.Area.Transparency);
            Console.WriteLine("Initial border transparency: " + series.Border.Transparency);

            // Modifica i valori di trasparenza
            series.Area.Transparency = 0.5; // 50% transparent
            series.Border.Transparency = 0.2; // 20% transparent

            Console.WriteLine("Modified area transparency: " + series.Area.Transparency);
            Console.WriteLine("Modified border transparency: " + series.Border.Transparency);

            // Salva la cartella di lavoro
            workbook.Save("AreaPropertyTransparencyDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


