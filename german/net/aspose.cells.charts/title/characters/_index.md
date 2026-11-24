---
title: "Title.Characters"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Title‑Methode. Gibt die Rich‑Text‑Formatierung dieses Titels zurück"
type: docs
url: /de/net/aspose.cells.charts/title/characters/
---
## Title.Characters method

Liest die Rich‑Text‑Formatierung dieses Titels.

```csharp
public FontSetting[] Characters()
```

### Rückgabewert

gibt ein FontSetting‑Array zurück

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apples");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Oranges");
            worksheet.Cells["B3"].PutValue(5);

            // Ein Diagramm erstellen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Diagrammtitel festlegen
            chart.Title.Text = "Fruit Sales Report";
            chart.Title.IsVisible = true;

            try
            {
                // Rufen Sie die Rich-Text-Formatierung des Titels ab
                FontSetting[] titleCharacters = chart.Title.Characters();
                
                // Ändern Sie die Schriftart des ersten Zeichens
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
            
            // Ergebnis speichern
            workbook.Save("TitleMethodCharactersDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


