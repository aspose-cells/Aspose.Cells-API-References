---
title: "Enum TextOrientationType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.TextOrientationType enum. Enumeriert Textorientierungstypen"
type: docs
url: /de/net/aspose.cells/textorientationtype/
---
## TextOrientationType enumeration

Enumeriert Textorientierungstypen.

```csharp
public enum TextOrientationType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| ClockWise | `0` | Dreht den Text um 90 Grad im Uhrzeigersinn. |
| CounterClockWise | `1` | Dreht den Text um 90 Grad gegen den Uhrzeigersinn. |
| NoRotation | `2` | Stellt den Standardwert dar. |
| TopToBottom | `3` | Zeigt Text von oben nach unten in der Zelle an. Gestapelter Text. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TextOrientationTypeDemo
    {
        public static void TextOrientationTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Hello, Aspose!");
            worksheet.Cells["A2"].PutValue("This is a test comment.");

            // Einen Kommentar zur Zelle A1 hinzufügen
            int commentIndex = worksheet.Comments.Add(0, 0);
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a comment with text orientation.";

            // Verschiedene Textorientierungstypen für den Kommentar festlegen
            comment.TextOrientationType = TextOrientationType.ClockWise;
            Console.WriteLine("Text Orientation: ClockWise");

            // Speichere die Arbeitsmappe
            workbook.Save("TextOrientationTypeExample_ClockWise.xlsx");

            // Textorientierung zu CounterClockWise ändern
            comment.TextOrientationType = TextOrientationType.CounterClockWise;
            Console.WriteLine("Text Orientation: CounterClockWise");

            // Speichere die Arbeitsmappe
            workbook.Save("TextOrientationTypeExample_CounterClockWise.xlsx");

            // Textorientierung zu NoRotation ändern
            comment.TextOrientationType = TextOrientationType.NoRotation;
            Console.WriteLine("Text Orientation: NoRotation");

            // Speichere die Arbeitsmappe
            workbook.Save("TextOrientationTypeExample_NoRotation.xlsx");

            // Textorientierung zu TopToBottom ändern
            comment.TextOrientationType = TextOrientationType.TopToBottom;
            Console.WriteLine("Text Orientation: TopToBottom");

            // Speichere die Arbeitsmappe
            workbook.Save("TextOrientationTypeExample_TopToBottom.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


