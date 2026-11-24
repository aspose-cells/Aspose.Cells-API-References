---
title: "MsoFillFormatHelper.Texture"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoFillFormatHelper-Eigenschaft. Gibt den Texturfülltyp zurück"
type: docs
url: /de/net/aspose.cells.drawing/msofillformathelper/texture/
---
## MsoFillFormatHelper.Texture property

Liest den Texturfülltyp.

```csharp
public TextureType Texture { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Reflection;

    public class MsoFillFormatHelperPropertyTextureDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Label hinzu, um das Beispiel sinnvoll zu machen
            worksheet.Cells["A1"].Value = "Texture Property Demo";

            try
            {
                // Erstelle eine Instanz von MsoFillFormatHelper mittels Reflexion (kein öffentlicher Konstruktor)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Zeige den aktuellen Wert der Texture-Eigenschaft an (schreibgeschützt)
                Console.WriteLine($"Current Texture type: {fillHelper.Texture}");

                // Demonstriere, dass die Eigenschaft schreibgeschützt ist, indem versucht wird, sie zu setzen (auskommentiert)
                // fillHelper.Texture = TextureType.Canvas; // Dies würde einen Kompilierungsfehler verursachen

                // Zeige alle verfügbaren Texturtypen als Referenz an
                Console.WriteLine("\nAvailable Texture Types:");
                foreach (TextureType textureType in Enum.GetValues(typeof(TextureType)))
                {
                    Console.WriteLine($"- {textureType}");
                }

                // Speichern Sie die Arbeitsmappe, um die erfolgreiche Ausführung zu demonstrieren
                workbook.Save("TextureDemo.xlsx");

                Console.WriteLine("\nTexture property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during Texture demo: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [TextureType](../../texturetype/)
* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


