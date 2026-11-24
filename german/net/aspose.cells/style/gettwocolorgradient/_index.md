---
title: "Style.GetTwoColorGradient"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Methode. Holen Sie die Einstellung für den Zweifarbverlauf"
type: docs
url: /de/net/aspose.cells/style/gettwocolorgradient/
---
## Style.GetTwoColorGradient method

Holen Sie die Einstellung für den Zweifarbverlauf.

```csharp
[Obsolete("Use Style.GetTwoColorGradientSetting() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void GetTwoColorGradient(out Color color1, out Color color2, 
    out GradientStyleType gradientStyleType, out int variant)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| color1 | Color& | Eine Gradientfarbe. |
| color2 | Color& | Zwei Gradientfarben. |
| gradientStyleType | GradientStyleType& | Gradient-Schattierungsstil. |
| Variante | Int32& | Die Gradientvariante. |

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode Style.GetTwoColorGradientSetting(). Diese Eigenschaft wird 12 Monate später, seit Dezember 2022, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class StyleMethodGetTwoColorGradientWithColorColorGradientStyleTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie einen Stil und setzen Sie einen Zweifarbverlauf
            Style style = workbook.CreateStyle();
            style.SetTwoColorGradient(Color.Red, Color.Blue, GradientStyleType.Horizontal, 1);

            // Wende den Stil auf eine Zelle an
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Two Color Gradient Demo");

            // Bereiten Sie Variablen vor, um die Gradient-Einstellungen zu erhalten
            Color color1 = Color.Empty;
            Color color2 = Color.Empty;
            GradientStyleType gradientStyle = GradientStyleType.Horizontal;
            int variant = 0;

            try
            {
                // Rufen Sie die Methode GetTwoColorGradient auf
#pragma warning disable CS0618 // Type or member is obsolete
                style.GetTwoColorGradient(out color1, out color2, out gradientStyle, out variant);
#pragma warning restore CS0618 // Type or member is obsolete

                // Zeigen Sie die abgerufenen Gradient-Einstellungen an
                Console.WriteLine("Gradient Settings:");
                Console.WriteLine($"Color1: {color1}");
                Console.WriteLine($"Color2: {color2}");
                Console.WriteLine($"Gradient Style: {gradientStyle}");
                Console.WriteLine($"Variant: {variant}");

                // Speichere die Arbeitsmappe
                workbook.Save("StyleMethodGetTwoColorGradientDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTwoColorGradient method: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [GradientStyleType](../../../aspose.cells.drawing/gradientstyletype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


