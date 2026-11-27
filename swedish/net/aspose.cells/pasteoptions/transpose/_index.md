---
title: "PasteOptions.Transpose"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PasteOptions-egenskap. Sant för att transponera rader och kolumner när området klistras in. Standardvärdet är Falskt"
type: docs
url: /sv/net/aspose.cells/pasteoptions/transpose/
---
## PasteOptions.Transpose property

Sant för att transponera rader och kolumner när området klistras in. Standardvärdet är Falskt.

```csharp
public bool Transpose { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyTransposeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Skapa källstil och tillämpa på horisontellt område
            Style style = workbook.CreateStyle();
            style.ForegroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            Aspose.Cells.Range sourceRange = cells.CreateRange(0, 0, 1, 4);
            sourceRange.SetStyle(style);

            // Skapa klistra-in-alternativ med transponering
            PasteOptions pasteOptions = new PasteOptions();
            pasteOptions.PasteType = PasteType.Formats;
            pasteOptions.Transpose = true;

            // Kopiera med transponering till vertikalt område
            Aspose.Cells.Range targetRange = cells.CreateRange(2, 0, 4, 1);
            targetRange.Copy(sourceRange, pasteOptions);

            // Spara arbetsboken
            workbook.Save("TransposeDemo.xlsx");
        }
    }
}
```

### Se även

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


