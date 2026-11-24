---
title: "Shape.FillFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt ein MsoFillFormat-Objekt zurück, das Füllformatierungseigenschaften für die angegebene Form enthält."
type: docs
url: /de/net/aspose.cells.drawing/shape/fillformat/
---
## Shape.FillFormat property

Gibt ein MsoFillFormat-Objekt zurück, das Füllformatierungseigenschaften für die angegebene Form enthält.

```csharp
[Obsolete("Use Shape.Fill property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoFillFormat FillFormat { get; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Shape.Fill-Eigenschaft. Diese Eigenschaft wird 12 Monate nach Juli 2016 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePropertyFillFormatDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie eine Rechteckform hinzu, um die FillFormat-Eigenschaft zu demonstrieren.
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 100);

            try
            {
                // Greifen Sie auf die FillFormat-Eigenschaft zu (schreibgeschützt).
                MsoFillFormat fillFormat = shape.FillFormat;

                // Aktuelle FillFormat-Eigenschaften anzeigen.
                Console.WriteLine("FillFormat ForeColor: " + fillFormat.ForeColor);
                Console.WriteLine("FillFormat Transparency: " + fillFormat.Transparency);
                Console.WriteLine("FillFormat BackColor: " + fillFormat.BackColor);
                Console.WriteLine("FillFormat IsVisible: " + fillFormat.IsVisible);

                // FillFormat-Eigenschaften ändern (da sie nicht schreibgeschützt sind).
                fillFormat.ForeColor = System.Drawing.Color.Red;
                fillFormat.Transparency = 0.5;
                fillFormat.BackColor = System.Drawing.Color.Yellow;
                fillFormat.IsVisible = true;

                // Aktualisierte FillFormat-Eigenschaften anzeigen.
                Console.WriteLine("Updated FillFormat ForeColor: " + fillFormat.ForeColor);
                Console.WriteLine("Updated FillFormat Transparency: " + fillFormat.Transparency);
                Console.WriteLine("Updated FillFormat BackColor: " + fillFormat.BackColor);
                Console.WriteLine("Updated FillFormat IsVisible: " + fillFormat.IsVisible);

                // Speichere die Arbeitsmappe
                workbook.Save("FillFormatDemo.xlsx");
                Console.WriteLine("FillFormat has been demonstrated and workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [MsoFillFormat](../../msofillformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


