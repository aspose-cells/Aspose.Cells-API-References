---
title: "Title.Characters"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Title. Ottiene la formattazione rich text di questo Titolo"
type: docs
url: /it/net/aspose.cells.charts/title/characters/
---
## Title.Characters method

Ottiene la formattazione del testo ricco di questo titolo.

```csharp
public FontSetting[] Characters()
```

### Valore di ritorno

restituisce un array FontSetting

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TitleMethodCharactersDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apples");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Oranges");
            worksheet.Cells["B3"].PutValue(5);

            // Crea un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Imposta titolo del grafico
            chart.Title.Text = "Fruit Sales Report";
            chart.Title.IsVisible = true;

            try
            {
                // Ottieni la formattazione del testo ricco del titolo
                FontSetting[] titleCharacters = chart.Title.Characters();
                
                // Modifica il carattere del primo carattere
                if (titleCharacters.Length > 0)
                {
                    titleCharacters[0].Font.Color = System.Drawing.Color.Red;
                    titleCharacters[0].Font.IsBold = true;
                    titleCharacters[0].Font.Size = 14;
                }

                Console.WriteLine("Characters method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Characters method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("TitleMethodCharactersDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


