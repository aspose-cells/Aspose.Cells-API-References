---
title: "TextureFill.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextureFill-Eigenschaft. Ruft den Texturtyp ab und setzt ihn."
type: docs
url: /de/net/aspose.cells.drawing/texturefill/type/
---
## TextureFill.Type property

Liest und setzt den Texturtyp

```csharp
public TextureType Type { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextureFillPropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Rechteckform hinzu, um die Texturfüllung zu demonstrieren
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 200);

            // Setze den Fülltyp auf Textur
            shape.Fill.FillType = FillType.Texture;

            // Auf die TextureFill-Eigenschaften zugreifen
            TextureFill textureFill = shape.Fill.TextureFill;

            try
            {
                // Den anfänglichen Type-Wert anzeigen
                Console.WriteLine("Initial Texture Type: " + textureFill.Type);

                // Einen anderen Texturtyp festlegen
                textureFill.Type = TextureType.Granite;
                Console.WriteLine("Updated Texture Type: " + textureFill.Type);

                // Einen anderen Texturtyp demonstrieren
                textureFill.Type = TextureType.WaterDroplets;
                Console.WriteLine("Final Texture Type: " + textureFill.Type);

                // Speichern Sie die Arbeitsmappe, um den Effekt zu sehen
                workbook.Save("TextureFillTypeDemo.xlsx");
                Console.WriteLine("Texture fill type demonstration completed successfully.");
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

* enum [TextureType](../../texturetype/)
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


