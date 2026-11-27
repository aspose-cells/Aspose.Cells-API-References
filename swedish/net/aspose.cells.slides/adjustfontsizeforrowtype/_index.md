---
title: "Enum AdjustFontSizeForRowType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Slides.AdjustFontSizeForRowType enum. Representerar vilken typ av rader som ska justeras"
type: docs
url: /sv/net/aspose.cells.slides/adjustfontsizeforrowtype/
---
## AdjustFontSizeForRowType enumeration

Representerar vilken typ av rader som bör justeras.

```csharp
public enum AdjustFontSizeForRowType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Ingen justering. |
| EmptyRows | `1` | Om raden är tom, ändra teckenstorlek så att den passar radens höjd. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i lite data i kalkylbladet
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Skapa en instans av PptxSaveOptions med inställningen AdjustFontSizeForRowType
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                AdjustFontSizeForRowType = AdjustFontSizeForRowType.EmptyRows
            };

            // Spara arbetsboken som en PPTX-fil
            workbook.Save("AdjustFontSizeForRowTypeDemo.pptx", saveOptions);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Slides](../../aspose.cells.slides/)
* assembly [Aspose.Cells](../../)


