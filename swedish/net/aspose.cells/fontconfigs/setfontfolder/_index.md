---
title: "FontConfigs.SetFontFolder"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontConfigs-metoden. Ställer in teckensnittsmappen"
type: docs
url: /sv/net/aspose.cells/fontconfigs/setfontfolder/
---
## FontConfigs.SetFontFolder method

Anger teckensnittsmappen

```csharp
public static void SetFontFolder(string fontFolder, bool recursive)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fontFolder | String | Mappen som innehåller TrueType-teckensnitt. |
| rekursiv | Boolean | Avgör om underkataloger ska skannas eller inte. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontConfigsMethodSetFontFolderWithStringBooleanDemo
    {
        public static void Run()
        {
            // Initiera en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite text i cell A1
            worksheet.Cells["A1"].PutValue("Sample Text with Custom Font");
            
            // Ange anpassad teckensnittsmapp och specificera om undermappar ska inkluderas
            FontConfigs.SetFontFolder("Fonts", true);
            
            // Applicera en teckensnittsstil som kan använda teckensnitt från den anpassade mappen
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "CustomFont"; // Assuming "CustomFont" exists in the Fonts folder
            style.Font.Size = 14;
            worksheet.Cells["A1"].SetStyle(style);
            
            // Spara arbetsboken som PDF
            workbook.Save("output.pdf", SaveFormat.Pdf);
        }
    }
}
```

### Se även

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


