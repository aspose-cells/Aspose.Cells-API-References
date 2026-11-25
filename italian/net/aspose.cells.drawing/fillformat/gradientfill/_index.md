---
title: "FillFormat.GradientFill"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FillFormat. Ottiene l'oggetto GradientFill"
type: docs
url: /it/net/aspose.cells.drawing/fillformat/gradientfill/
---
## FillFormat.GradientFill property

Ottiene l'oggetto `GradientFill`.

```csharp
public GradientFill GradientFill { get; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientFillDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fornisci alcuni dati per un grafico
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico a colonne
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Accedi al formato di riempimento dell'area della prima serie
                FillFormat fillFormat = chart.NSeries[0].Area.FillFormat;

                // Applica un gradiente a due colori alla serie
                fillFormat.SetTwoColorGradient(Color.Red, Color.Blue,
                                               GradientStyleType.Horizontal, 2);

                // Recupera l'oggetto GradientFill (proprietà di sola lettura)
                GradientFill gradientFill = fillFormat.GradientFill;

                // Visualizza alcune informazioni sul riempimento a gradiente
                Console.WriteLine("GradientFill details:");
                Console.WriteLine($"  FillType      : {gradientFill.FillType}");
                Console.WriteLine($"  DirectionType: {gradientFill.DirectionType}");
                Console.WriteLine($"  Angle         : {gradientFill.Angle}");

                // Modifica opzionalmente l'angolo del gradiente usando l'accessore set
                gradientFill.Angle = 45.0f;
                Console.WriteLine($"  New Angle set to: {gradientFill.Angle}");

                // Salva la cartella di lavoro
                workbook.Save("FillFormatGradientFillDemo.xlsx");
                Console.WriteLine("Workbook saved as FillFormatGradientFillDemo.xlsx");
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

* class [GradientFill](../../gradientfill/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


