---
title: "FontConfigs.SetFontFolders"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontConfigs-metoden. Ställer in teckensnittsmappen"
type: docs
url: /sv/net/aspose.cells/fontconfigs/setfontfolders/
---
## FontConfigs.SetFontFolders method

Anger teckensnittsmappen

```csharp
public static void SetFontFolders(string[] fontFolders, bool recursive)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fontFolders | String[] | Mapparna som innehåller TrueType-teckensnitt. |
| rekursiv | Boolean | Avgör om underkataloger ska skannas eller inte. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodSetFontFoldersWithStringBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange lite text som kommer att använda anpassade teckensnitt
            worksheet.Cells["A1"].PutValue("Text with custom font");

            // Förbered teckensnittsmappar (ersätt med faktiska sökvägar på ditt system)
            string[] fontFolders = new string[] 
            {
                @"C:\Windows\Fonts",
                @"D:\CustomFonts"
            };
            bool recursiveSearch = true;

            try
            {
                // Anropa SetFontFolders-metoden med String[] och Boolean-parameterar
                FontConfigs.SetFontFolders(fontFolders, recursiveSearch);

                // Applicera ett teckensnitt som kan finnas i någon av dessa mappar
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = "SomeCustomFont"; // Replace with actual font name
                worksheet.Cells["A1"].SetStyle(style);

                Console.WriteLine("Font folders set successfully. Workbook may use fonts from these locations.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting font folders: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("FontConfigsSetFontFoldersDemo.xlsx");
        }
    }
}
```

### Se även

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


