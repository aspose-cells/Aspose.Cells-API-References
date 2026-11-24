---
title: "Shape.FormatCharacters"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Methode. Formatiert einige Zeichen mit den Schriftarteinstellungen"
type: docs
url: /de/net/aspose.cells.drawing/shape/formatcharacters/
---
## Shape.FormatCharacters method

Formatiert einige Zeichen mit den Schriftarteinstellungen.

```csharp
public void FormatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startIndex | Int32 | Der Startindex. |
| Länge | Int32 | Die Länge. |
| Schriftart | Schriftart | Die Schriftarteinstellung. |
| Flag | StyleFlag | Das Flag der Schriftarteinstellung. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodFormatCharactersWithInt32Int32FontStyleFlagDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge ein Textfeld zum Arbeitsblatt hinzu
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            textBox.Text = "Sample Text Formatting";
            
            // Erstelle eine Schriftart mit den gewünschten Eigenschaften
            Aspose.Cells.Font font = textBox.Font;
            font.Name = "Arial";
            font.Size = 12;
            font.IsBold = true;
            
            // Erstelle ein Stil-Flag, um anzugeben, welche Eigenschaften angewendet werden sollen
            StyleFlag flag = new StyleFlag();
            flag.FontName = true;
            flag.FontSize = true;
            flag.FontBold = true;
            
            // Formatierung auf bestimmte Zeichen anwenden
            textBox.FormatCharacters(0, 6, font, flag);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Font](../../../aspose.cells/font/)
* class [StyleFlag](../../../aspose.cells/styleflag/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


