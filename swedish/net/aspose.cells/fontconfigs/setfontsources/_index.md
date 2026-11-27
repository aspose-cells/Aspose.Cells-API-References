---
title: "FontConfigs.SetFontSources"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontConfigs-metoden. Ställer in teckensnittskällorna"
type: docs
url: /sv/net/aspose.cells/fontconfigs/setfontsources/
---
## FontConfigs.SetFontSources method

Anger teckensnittskällorna.

```csharp
public static void SetFontSources(FontSourceBase[] sources)
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

    public class FontConfigsMethodSetFontSourcesWithFontSourceBaseDemo
    {
        public static void Run()
        {
            // Skapa en temporär teckensnittfil för demonstration
            string tempFontFile = Path.Combine(Path.GetTempPath(), "testfont.ttf");
            try
            {
                File.WriteAllBytes(tempFontFile, new byte[0]); // Empty file for demo

                // Skapa teckensnittskällor
                FontSourceBase[] fontSources = new FontSourceBase[]
                {
                    new FolderFontSource(Path.GetTempPath(), true),
                    new FileFontSource(tempFontFile)
                };

                try
                {
                    // Anropa SetFontSources-metoden
                    FontConfigs.SetFontSources(fontSources);

                    // Verifiera att teckensnittskällorna har ställts in
                    FontSourceBase[] currentSources = FontConfigs.GetFontSources();
                    Console.WriteLine($"Font sources set successfully. Count: {currentSources.Length}");

                    // Demonstrera effekten genom att kontrollera om ett teckensnitt är tillgängligt
                    bool isAvailable = FontConfigs.IsFontAvailable("Arial");
                    Console.WriteLine($"Is Arial available: {isAvailable}");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error executing SetFontSources method: {ex.Message}");
                }
            }
            finally
            {
                // Rensa upp
                if (File.Exists(tempFontFile))
                {
                    File.Delete(tempFontFile);
                }
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


