---
title: "IndividualFontConfigs.SetFontFolder"
second_title: "Aspose.Cells för .NET API‑referens"
description: "IndividualFontConfigs-metod. Anger teckensnittsmappen"
type: docs
url: /sv/net/aspose.cells/individualfontconfigs/setfontfolder/
---
## IndividualFontConfigs.SetFontFolder method

Anger teckensnittsmappen

```csharp
public void SetFontFolder(string fontFolder, bool recursive)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fontFolder | String | Mappen som innehåller TrueType-teckensnitt. |
| rekursiv | Boolean | Avgör om underkataloger ska skannas eller inte. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodSetFontFolderWithStringBooleanDemo
    {
        public static void Run()
        {
            // Skapa en instans av IndividualFontConfigs
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();
            
            // Ange sökvägen till teckensnittsmappen och om sökningen ska vara rekursiv
            string fontFolderPath = @"C:\Windows\Fonts";
            bool recursiveSearch = true;

            try
            {
                // Anropa SetFontFolder med de angivna parametrarna
                fontConfigs.SetFontFolder(fontFolderPath, recursiveSearch);
                
                Console.WriteLine($"Successfully set font folder to: {fontFolderPath}");
                Console.WriteLine($"Recursive search enabled: {recursiveSearch}");

                // Skapa en arbetsbok för att demonstrera teckensnittsanvändning
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Ange en stil som kan använda teckensnitt från den angivna mappen
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial"; // Assuming Arial exists in the font folder
                style.Font.Size = 12;
                
                worksheet.Cells["A1"].Value = "Text with font from specified folder";
                worksheet.Cells["A1"].SetStyle(style);
                
                // Spara arbetsboken
                workbook.Save("FontConfigDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting font folder: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


