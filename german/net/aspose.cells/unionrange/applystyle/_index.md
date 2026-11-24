---
title: "UnionRange.ApplyStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "UnionRange-Methode. Wendet Formate für einen gesamten Bereich an"
type: docs
url: /de/net/aspose.cells/unionrange/applystyle/
---
## UnionRange.ApplyStyle method

Wendet Formate für einen gesamten Bereich an.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stil | Stil | Das Stil‑Objekt, das angewendet wird. |
| Flag | StyleFlag | Flags, die die angewendeten Formatierungseigenschaften angeben. |

### Hinweise

Jede Zelle in diesem Bereich enthält ein [`Style`](../../style/)-Objekt. Daher ist dies eine speicherintensive Methode. Bitte verwenden Sie sie vorsichtig.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class UnionRangeMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle einen Union-Bereich, der die Zellen A1 bis B2 abdeckt
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

            // Füge einige Daten für den Kontext hinzu
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B2"].Value = "More Data";

            try
            {
                // Erstelle einen Stil mit spezifischer Formatierung
                Style style = workbook.CreateStyle();
                style.Font.IsBold = true;
                style.Font.Color = Color.Red;
                style.ForegroundColor = Color.LightBlue;
                style.Pattern = BackgroundType.Solid;
                style.HorizontalAlignment = TextAlignmentType.Center;

                // Erstelle ein StyleFlag, um anzugeben, welche Eigenschaften angewendet werden sollen
                StyleFlag flag = new StyleFlag();
                flag.FontBold = true;
                flag.FontColor = true;
                flag.CellShading = true;
                flag.HorizontalAlignment = true;

                // Rufe ApplyStyle mit den Stil- und Flag-Parametern auf
                unionRange.ApplyStyle(style, flag);

                Console.WriteLine("ApplyStyle method called successfully");
                Console.WriteLine($"Applied style to range: {unionRange.RefersTo}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ApplyStyle: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("UnionRangeMethodApplyStyleWithStyleStyleFlagDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


