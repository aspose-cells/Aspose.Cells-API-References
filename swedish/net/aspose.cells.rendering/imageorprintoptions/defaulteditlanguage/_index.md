---
title: "ImageOrPrintOptions.DefaultEditLanguage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions‑egenskap. Hämtar eller anger standardspråk för redigering"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/defaulteditlanguage/
---
## ImageOrPrintOptions.DefaultEditLanguage property

Hämtar eller anger standardspråket för redigering.

```csharp
public DefaultEditLanguage DefaultEditLanguage { get; set; }
```

### Anmärkningar

Den kan visa/rendera olika layouter för textparagraf när olika redigeringsspråk är inställda. Standard är Auto.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyDefaultEditLanguageDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ställ in arbetsbokens standardsnitt till ett som stöder CJK‑tecken
            workbook.DefaultStyle.Font.Name = "MS Gothic";
            
            // Ange japansk text som kräver korrekt radbrytning
            string japaneseText = "日本語のテキストサンプル：これは折り返し表示のテストです。長いテキストをセル内で適切に表示するか確認します。";
            sheet.Cells["A1"].Value = japaneseText;
            
            // Konfigurera cellformatering – fixad med korrekt egenskapsnamn
            Cell cell = sheet.Cells["A1"];
            Style style = cell.GetStyle();
            style.IsTextWrapped = true;  // Correct property name for text wrapping
            cell.SetStyle(style);
            
            sheet.Cells.SetColumnWidth(0, 15);
            sheet.Cells.SetRowHeight(0, 60);

            // Skapa alternativ för bildrendering
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.DefaultEditLanguage = DefaultEditLanguage.CJK;
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.CheckWorkbookDefaultFont = true;

            // Rendera kalkylbladet till bild
            SheetRender renderer = new SheetRender(sheet, options);
            renderer.ToImage(0, "CJK_Text_Rendering.png");
            
            Console.WriteLine("Generated image with CJK text rendering.");
        }
    }
}
```

### Se även

* enum [DefaultEditLanguage](../../../aspose.cells/defaulteditlanguage/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


