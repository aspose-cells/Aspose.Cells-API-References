---
title: "IndividualFontConfigs.GetFontSources"
second_title: "Aspose.Cells för .NET API‑referens"
description: "IndividualFontConfigs-metod. Hämtar en kopia av arrayen som innehåller listan över källor"
type: docs
url: /sv/net/aspose.cells/individualfontconfigs/getfontsources/
---
## IndividualFontConfigs.GetFontSources method

Hämtar en kopia av arrayen som innehåller listan över källor

```csharp
public FontSourceBase[] GetFontSources()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodGetFontSourcesDemo
    {
        public static void Run()
        {
            // Skapa individuella teckensnittskonfigurationer
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Ange några teckensnittskällor (mappar som innehåller teckensnitt)
            string fontFolder1 = @"C:\Windows\Fonts";
            string fontFolder2 = @"D:\CustomFonts";
            fontConfigs.SetFontFolder(fontFolder1, false);
            fontConfigs.SetFontFolder(fontFolder2, true);

            try
            {
                // Hämta de aktuella teckensnittskällorna
                FontSourceBase[] fontSources = fontConfigs.GetFontSources();

                Console.WriteLine("Current font sources:");
                foreach (var source in fontSources)
                {
                    if (source is FolderFontSource folderSource)
                    {
                        Console.WriteLine($"- Folder: {folderSource.FolderPath} (Recursive: {folderSource.ScanSubFolders})");
                    }
                }

                // Skapa en arbetsbok för att demonstrera effekten
                Workbook workbook = new Workbook(FileFormatType.Xlsx);
                // Använd teckensnittskonfigurationerna när du skapar stilar eller arbetar med teckensnitt
                // (Arbetsboken har ingen FontConfigs-egenskap, så vi tar bort den raden)
                Worksheet worksheet = workbook.Worksheets[0];

                // Använd ett anpassat teckensnitt som kan finnas i någon av mapparna
                Style style = workbook.CreateStyle();
                style.Font.Name = "SomeCustomFont";
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].PutValue("Text with custom font");

                Console.WriteLine("Workbook created with custom font configurations.");
                workbook.Save("MethodGetFontSourcesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFontSources method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [FontSourceBase](../../fontsourcebase/)
* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


