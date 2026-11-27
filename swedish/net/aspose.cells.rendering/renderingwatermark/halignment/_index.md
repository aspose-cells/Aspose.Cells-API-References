---
title: "RenderingWatermark.HAlignment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RenderingWatermark-egenskap. Hämtar eller anger horisontell justering av vattenstämpeln på sidan"
type: docs
url: /sv/net/aspose.cells.rendering/renderingwatermark/halignment/
---
## RenderingWatermark.HAlignment property

Hämtar eller anger horisontell justering av vattenstämpeln på sidan.

```csharp
public TextAlignmentType HAlignment { get; set; }
```

### Anmärkningar

Endast Left, Center, Right är giltiga. Standard är Left.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyHAlignmentDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Watermark HAlignment Demo");

            // Skapa PDF-sparalternativ
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Skapa och konfigurera vattenstämpel med olika HAlignment-inställningar
            RenderingFont font = new RenderingFont("Arial", 48)
            {
                Bold = true,
                Color = System.Drawing.Color.Blue
            };

            // Skapa vattenstämpel med Center-justering
            RenderingWatermark watermark = new RenderingWatermark("CENTER ALIGNED", font)
            {
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                Opacity = 0.5f
            };
            pdfSaveOptions.Watermark = watermark;

            // Spara med centerjusterad vattenstämpel
            workbook.Save("WatermarkCenterAlignment.pdf", pdfSaveOptions);

            // Ändra till Left-justering
            watermark.HAlignment = TextAlignmentType.Left;
            workbook.Save("WatermarkLeftAlignment.pdf", pdfSaveOptions);

            // Ändra till Right-justering
            watermark.HAlignment = TextAlignmentType.Right;
            workbook.Save("WatermarkRightAlignment.pdf", pdfSaveOptions);
        }
    }
}
```

### Se även

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


