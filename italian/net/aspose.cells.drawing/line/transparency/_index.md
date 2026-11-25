---
title: "Line.Transparency"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Line. Restituisce o imposta il grado di trasparenza della linea come valore da 0.0 opaco a 1.0 trasparente"
type: docs
url: /it/net/aspose.cells.drawing/line/transparency/
---
## Line.Transparency property

Restituisce o imposta il grado di trasparenza della linea come valore da 0,0 (opaco) a 1,0 (trasparente).

```csharp
public double Transparency { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class LinePropertyTransparencyDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Crea un foglio di lavoro di esempio
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati per rendere l'esempio significativo
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B1"].PutValue("Values");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            try
            {
                // Aggiungi un grafico a linee per dimostrare le proprietà della linea
                int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("A1:B3", true);

                // Ottieni le proprietà della linea dal bordo della serie del grafico
                Line line = chart.NSeries[0].Border;

                // Visualizza il valore corrente di Transparency
                Console.WriteLine("Current Transparency: " + line.Transparency);

                // Imposta un nuovo valore di Transparency (0.0 = opaco, 1.0 = trasparente)
                line.Transparency = 0.5;
                Console.WriteLine("Updated Transparency: " + line.Transparency);

                // Salva la cartella di lavoro
                workbook.Save("TransparencyDemo.xlsx");
                Console.WriteLine("Transparency property demonstrated successfully.");
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

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


