---
title: "FontConfigs.GetFontSources"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FontConfigs-Methode. Gibt eine Kopie des Arrays zurück, das die Liste der Quellen enthält."
type: docs
url: /de/net/aspose.cells/fontconfigs/getfontsources/
---
## FontConfigs.GetFontSources method

Gibt eine Kopie des Arrays zurück, das die Liste der Quellen enthält

```csharp
public static FontSourceBase[] GetFontSources()
```

### Beispiele

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
                // Rufen Sie die aktuellen Schriftquellen ab.
                FontSourceBase[] fontSources = FontConfigs.GetFontSources();

                // Zeigen Sie Informationen zu jeder Schriftquelle an.
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

                // Erstellen Sie ein neues Arbeitsbuch, um die Wirkung zu demonstrieren.
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Legen Sie einen Text mit einer Schriftart fest, die diese Quellen verwenden könnte.
                worksheet.Cells["A1"].PutValue("Font Sources Demo");
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                worksheet.Cells["A1"].SetStyle(style);

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [FontSourceBase](../../fontsourcebase/)
* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


