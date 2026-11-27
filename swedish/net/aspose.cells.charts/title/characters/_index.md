---
title: "Title.Characters"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Title‑metod. Hämtar rik textformatering för denna titel"
type: docs
url: /sv/net/aspose.cells.charts/title/characters/
---
## Title.Characters method

Hämtar rik textformatering för den här titeln.

```csharp
public FontSetting[] Characters()
```

### Returvärde

returnerar FontSetting‑array

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i arbetsbladet
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apples");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Oranges");
            worksheet.Cells["B3"].PutValue(5);

            // Skapa ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Ange diagramtitel
            chart.Title.Text = "Fruit Sales Report";
            chart.Title.IsVisible = true;

            try
            {
                // Hämta den riktextformateringen för titeln
                FontSetting[] titleCharacters = chart.Title.Characters();
                
                // Ändra det första tecknets teckensnitt
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
            
            // Spara resultatet
            workbook.Save("TitleMethodCharactersDemo.xlsx");
        }
    }
}
```

### Se även

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


