---
title: "DisplayUnitLabel.Font"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DisplayUnitLabel property. Gibt ein Font-Objekt des angegebenen ChartFrame-Objekts zurück"
type: docs
url: /de/net/aspose.cells.charts/displayunitlabel/font/
---
## DisplayUnitLabel.Font property

Gibt ein `Font`-Objekt des angegebenen ChartFrame-Objekts zurück.

```csharp
public override Font Font { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class DisplayUnitLabelPropertyFontDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue(1000);
            worksheet.Cells["A2"].PutValue(2000);
            worksheet.Cells["A3"].PutValue(3000);
            worksheet.Cells["A4"].PutValue(4000);
            worksheet.Cells["A5"].PutValue(5000);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A5", true);

            // Anzeigeeinheiten für die Werteachse festlegen
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;
            chart.ValueAxis.DisplayUnitLabel.Text = "Thousands";

            // Hole die DisplayUnitLabel-Instanz
            DisplayUnitLabel displayUnitLabel = chart.ValueAxis.DisplayUnitLabel;

            // Aktuelle Font-Eigenschaften anzeigen
            Font currentFont = displayUnitLabel.Font;
            Console.WriteLine("Current Font Properties:");
            Console.WriteLine($"Name: {currentFont.Name}");
            Console.WriteLine($"Size: {currentFont.Size}");
            Console.WriteLine($"Color: {currentFont.Color}");
            Console.WriteLine($"Bold: {currentFont.IsBold}");
            Console.WriteLine($"Italic: {currentFont.IsItalic}");

            // Erstelle einen neuen Schriftstil und wende ihn auf das Anzeigeeinheiten-Label an
            // Hinweis: Da Font schreibgeschützt ist, ändern wir seine Eigenschaften direkt
            currentFont.Name = "Arial";
            currentFont.Size = 12;
            currentFont.Color = System.Drawing.Color.Red;
            currentFont.IsBold = true;
            currentFont.IsItalic = false;
            currentFont.Underline = FontUnderlineType.Single;

            // Speichere die Arbeitsmappe, um die Änderungen zu sehen
            workbook.Save("DisplayUnitLabelFontDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Font](../../../aspose.cells/font/)
* class [DisplayUnitLabel](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


