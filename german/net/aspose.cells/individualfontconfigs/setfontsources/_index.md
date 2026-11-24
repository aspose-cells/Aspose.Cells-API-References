---
title: "IndividualFontConfigs.SetFontSources"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "IndividualFontConfigs-Methode. Legt die Schriftquellen fest"
type: docs
url: /de/net/aspose.cells/individualfontconfigs/setfontsources/
---
## IndividualFontConfigs.SetFontSources method

Legt die Schriftquellen fest.

```csharp
public void SetFontSources(FontSourceBase[] sources)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Quellen | FontSourceBase[] | Ein Array von Quellen, das TrueType-Schriften enthält. |

### Beispiele

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
            // Erstelle individuelle Schriftkonfigurationen
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Bereite Schriftquellen vor – unter Verwendung von Ordner- und Speicher-Schriftquellen
            FontSourceBase[] fontSources = new FontSourceBase[]
            {
                new FolderFontSource(@"C:\Windows\Fonts", false),
                new MemoryFontSource(File.ReadAllBytes(@"C:\Windows\Fonts\arial.ttf"))
            };

            try
            {
                // Rufe SetFontSources mit den vorbereiteten Schriftquellen auf
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

                // Erstelle eine Arbeitsmappe, um den Effekt zu demonstrieren
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Verwende eine Schrift, die aus den Quellen verfügbar sein sollte
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].Value = "Text using font from custom sources";
                worksheet.Cells["A2"].Value = "This demonstrates SetFontSources with FontSourceBase[]";

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [FontSourceBase](../../fontsourcebase/)
* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


