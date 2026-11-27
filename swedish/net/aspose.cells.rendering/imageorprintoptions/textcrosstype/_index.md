---
title: "ImageOrPrintOptions.TextCrossType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Hämtar eller anger visningstyp för text när textbredden är större än cellbredden."
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/textcrosstype/
---
## ImageOrPrintOptions.TextCrossType property

Hämtar eller anger visningstyp för text när textbredden är större än cellbredden.

```csharp
public TextCrossType TextCrossType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyTextCrossTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange lång text som kommer att överskrida cellbredden
            worksheet.Cells["A1"].PutValue("This is a long text that exceeds cell width");
            worksheet.Cells["A1"].GetStyle().ShrinkToFit = false;

            // Skapa bild- eller utskriftsalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Demonstrera olika TextCrossType-inställningar
            options.TextCrossType = TextCrossType.Default;
            SaveAsImage(workbook, options, "TextCrossType_Default.png");

            options.TextCrossType = TextCrossType.CrossKeep;
            SaveAsImage(workbook, options, "TextCrossType_CrossKeep.png");

            options.TextCrossType = TextCrossType.CrossOverride;
            SaveAsImage(workbook, options, "TextCrossType_CrossOverride.png");

            options.TextCrossType = TextCrossType.StrictInCell;
            SaveAsImage(workbook, options, "TextCrossType_StrictInCell.png");
        }

        private static void SaveAsImage(Workbook workbook, ImageOrPrintOptions options, string fileName)
        {
            SheetRender sr = new SheetRender(workbook.Worksheets[0], options);
            sr.ToImage(0, fileName);
        }
    }
}
```

### Se även

* enum [TextCrossType](../../../aspose.cells/textcrosstype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


