---
title: "IndividualFontConfigs.SetFontSources"
second_title: "Aspose.Cells för .NET API‑referens"
description: "IndividualFontConfigs-metod. Anger teckensnittskällorna"
type: docs
url: /sv/net/aspose.cells/individualfontconfigs/setfontsources/
---
## IndividualFontConfigs.SetFontSources method

Anger teckensnittskällorna.

```csharp
public void SetFontSources(FontSourceBase[] sources)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| källor | FontSourceBase[] | En array av källor som innehåller TrueType-teckensnitt. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class IndividualFontConfigsMethodSetFontSourcesWithFontSourceBaseDemo
    {
        public static void Run()
        {
            // Skapa individuella teckensnittskonfigurationer
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Förbered teckensnittskällor - med både mapp- och minneskällor för teckensnitt
            FontSourceBase[] fontSources = new FontSourceBase[]
            {
                new FolderFontSource(@"C:\Windows\Fonts", false),
                new MemoryFontSource(File.ReadAllBytes(@"C:\Windows\Fonts\arial.ttf"))
            };

            try
            {
                // Anropa SetFontSources med de förberedda teckensnittskällorna
                fontConfigs.SetFontSources(fontSources);

                Console.WriteLine("Font sources set successfully:");
                foreach (var source in fontConfigs.GetFontSources())
                {
                    if (source is FolderFontSource folderSource)
                    {
                        Console.WriteLine($"- Folder: {folderSource.FolderPath} (Recursive: {folderSource.ScanSubFolders})");
                    }
                    else if (source is MemoryFontSource memorySource)
                    {
                        Console.WriteLine($"- Memory font with data length: {memorySource.FontData.Length} bytes");
                    }
                }

                // Skapa en arbetsbok för att demonstrera effekten
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Använd ett teckensnitt som bör vara tillgängligt från källorna
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].Value = "Text using font from custom sources";
                worksheet.Cells["A2"].Value = "This demonstrates SetFontSources with FontSourceBase[]";

                // Spara arbetsboken
                workbook.Save("SetFontSourcesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFontSources method: {ex.Message}");
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


