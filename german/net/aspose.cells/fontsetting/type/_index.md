---
title: "FontSetting.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FontSetting-Eigenschaft. Gibt den Typ des Textknotens zurück"
type: docs
url: /de/net/aspose.cells/fontsetting/type/
---
## FontSetting.Type property

Ermittelt den Typ des Textknotens.

```csharp
public virtual TextNodeType Type { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;  // Added this using directive
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingPropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Text zu einer Zelle hinzu
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Rufen Sie die Schriftarteinstellungen für die Zeichen der Zelle ab
            FontSetting fontSetting = new FontSetting(0, 6, workbook.Worksheets);

            // Aktuellen Type-Wert anzeigen
            Console.WriteLine("Current Type value: " + fontSetting.Type);

            // Demonstrieren Sie, wie Type die Textverarbeitung beeinflusst
            if (fontSetting.Type == TextNodeType.TextRun)
            {
                Console.WriteLine("The text is a standard text run.");
            }
            else if (fontSetting.Type == TextNodeType.TextParagraph)
            {
                Console.WriteLine("The text is part of a paragraph.");
            }
            else if (fontSetting.Type == TextNodeType.Equation)
            {
                Console.WriteLine("The text represents an equation.");
            }

            // Wenden Sie unterschiedliche Formatierungen basierend auf Type an
            if (fontSetting.Type == TextNodeType.TextRun)
            {
                fontSetting.Font.Color = System.Drawing.Color.Red;
                fontSetting.SetWordArtStyle(PresetWordArtStyle.WordArtStyle1);
            }

            // Ergebnis speichern
            workbook.Save("FontSettingTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TextNodeType](../../../aspose.cells.drawing.texts/textnodetype/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


