---
title: "Enum AdjustFontSizeForRowType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Slides.AdjustFontSizeForRowType enum. Gibt an, welche Art von Zeilen angepasst werden soll."
type: docs
url: /de/net/aspose.cells.slides/adjustfontsizeforrowtype/
---
## AdjustFontSizeForRowType enumeration

Stellt dar, welche Art von Zeilen angepasst werden sollten.

```csharp
public enum AdjustFontSizeForRowType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Keine Anpassung. |
| EmptyRows | `1` | Wenn die Zeile leer ist, die Schriftgröße ändern, damit sie zur Zeilenhöhe passt. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;

namespace AsposeCellsExamples
{
    public class SlidesClassAdjustFontSizeForRowTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füllen Sie einige Daten in das Arbeitsblatt ein
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Erstellen Sie eine Instanz von PptxSaveOptions mit der Einstellung AdjustFontSizeForRowType.
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                AdjustFontSizeForRowType = AdjustFontSizeForRowType.EmptyRows
            };

            // Speichere die Arbeitsmappe als PPTX‑Datei
            workbook.Save("AdjustFontSizeForRowTypeDemo.pptx", saveOptions);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Slides](../../aspose.cells.slides/)
* assembly [Aspose.Cells](../../)


