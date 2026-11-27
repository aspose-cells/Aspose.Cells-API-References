---
title: "FontConfigs.GetFontSources"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontConfigs-metod. Hämtar en kopia av arrayen som innehåller listan över källor"
type: docs
url: /sv/net/aspose.cells/fontconfigs/getfontsources/
---
## FontConfigs.GetFontSources method

Hämtar en kopia av arrayen som innehåller listan över källor

```csharp
public static FontSourceBase[] GetFontSources()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodGetFontSourcesDemo
    {
        public static void Run()
        {
            try
            {
                // Hämta de aktuella teckensnittskällorna
                FontSourceBase[] fontSources = FontConfigs.GetFontSources();

                // Visa information om varje teckensnittskälla
                if (fontSources != null)
                {
                    Console.WriteLine("Current font sources:");
                    foreach (var source in fontSources)
                    {
                        Console.WriteLine($"Type: {source.GetType().Name}");
                        if (source is FolderFontSource folderSource)
                        {
                            Console.WriteLine($"Folder path: {folderSource.FolderPath}");
                            Console.WriteLine($"Scan subfolders: {folderSource.ScanSubFolders}");
                        }
                        else if (source is FileFontSource fileSource)
                        {
                            Console.WriteLine($"File path: {fileSource.FilePath}");
                        }
                        else if (source is MemoryFontSource memorySource)
                        {
                            Console.WriteLine($"Font data present: {memorySource.FontData != null}");
                        }
                        Console.WriteLine();
                    }
                }
                else
                {
                    Console.WriteLine("No font sources are currently set.");
                }

                // Skapa en ny arbetsbok för att demonstrera effekten
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Ange lite text med ett teckensnitt som kan använda dessa källor
                worksheet.Cells["A1"].PutValue("Font Sources Demo");
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                worksheet.Cells["A1"].SetStyle(style);

                // Spara arbetsboken
                workbook.Save("FontConfigsGetFontSourcesDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while working with font sources: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [FontSourceBase](../../fontsourcebase/)
* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


