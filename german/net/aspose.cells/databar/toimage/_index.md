---
title: "DataBar.ToImage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataBar-Methode. Rendern Sie die Datenleiste in einer Zelle in ein Bild-Byte-Array"
type: docs
url: /de/net/aspose.cells/databar/toimage/
---
## DataBar.ToImage method

Rendert den Datenbalken in einer Zelle zu einem Bild‑Byte‑Array.

```csharp
public byte[] ToImage(Cell cell, ImageOrPrintOptions imgOpts)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zelle | Zelle | Geben Sie an, in welcher Zelle die Datenleiste gerendert werden soll |
| imgOpts | ImageOrPrintOptions | ImageOrPrintOptions enthält einige Eigenschaften des Ausgabebildes |

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class DataBarMethodToImageWithCellImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten und bedingte Formatierung hinzufügen
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            
            // Bedingte Formatierung für Datenbalken hinzufügen
            int idx = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[idx];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            fcc.AddArea(area);
            
            idx = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = fcc[idx];
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.Min;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.Max;
            
            // Abrufen Sie die Zelle mit bedingter Formatierung
            Cell cell = worksheet.Cells["A1"];
            ConditionalFormattingResult result = cell.GetConditionalFormattingResult();
            
            if (result != null && result.ConditionalFormattingDataBar != null)
            {
                DataBar bar = result.ConditionalFormattingDataBar;
                ImageOrPrintOptions imgOpts = new ImageOrPrintOptions();
                
                // Konvertieren Sie die Datenleiste in ein Bild
                byte[] img = bar.ToImage(cell, imgOpts);
                
                // Speichern Sie das Bild
                string outputPath = "DataBarImage.png";
                File.WriteAllBytes(outputPath, img);
                
                // Für die Bildüberprüfung müssen Sie das Paket System.Drawing.Common hinzufügen
                // und verwenden Sie System.Drawing.Image bei Bedarf
                Console.WriteLine($"Data bar image saved to {outputPath}");
            }
        }
    }
}
```

### Siehe auch

* class [Cell](../../cell/)
* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


