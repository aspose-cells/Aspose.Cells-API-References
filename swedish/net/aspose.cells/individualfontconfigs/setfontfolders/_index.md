---
title: "IndividualFontConfigs.SetFontFolders"
second_title: "Aspose.Cells för .NET API‑referens"
description: "IndividualFontConfigs-metod. Anger teckensnittsmapparna"
type: docs
url: /sv/net/aspose.cells/individualfontconfigs/setfontfolders/
---
## IndividualFontConfigs.SetFontFolders method

Ställer in teckensnittsmapparna

```csharp
public void SetFontFolders(string[] fontFolders, bool recursive)
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

    public class IndividualFontConfigsMethodSetFontFoldersWithStringBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en instans av IndividualFontConfigs
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Förbered array med teckensnittsmappar
            string[] fontFolders = new string[] { @"C:\Windows\Fonts", @"D:\CustomFonts" };
            bool recursiveSearch = true;

            try
            {
                // Anropa SetFontFolders-metoden med String[] och Boolean-parameterar
                fontConfigs.SetFontFolders(fontFolders, recursiveSearch);

                // Demonstrera effekten genom att använda ett anpassat teckensnitt
                worksheet.Cells["A1"].PutValue("Text with custom font");
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = "SomeCustomFont"; // Assuming this font exists in one of the folders
                worksheet.Cells["A1"].SetStyle(style);

                Console.WriteLine("SetFontFolders method executed successfully with parameters (String[], Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFontFolders method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("SetFontFoldersDemo.xlsx");
        }
    }
}
```

### Se även

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


