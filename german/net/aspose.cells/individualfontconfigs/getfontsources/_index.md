---
title: "IndividualFontConfigs.GetFontSources"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "IndividualFontConfigs-Methode. Gibt eine Kopie des Arrays zurück, das die Liste der Quellen enthält"
type: docs
url: /de/net/aspose.cells/individualfontconfigs/getfontsources/
---
## IndividualFontConfigs.GetFontSources method

Gibt eine Kopie des Arrays zurück, das die Liste der Quellen enthält

```csharp
public FontSourceBase[] GetFontSources()
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodGetFontSourcesDemo
    {
        public static void Run()
        {
            // Erstelle individuelle Schriftkonfigurationen
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Lege einige Schriftquellen fest (Ordner, die Schriften enthalten)
            string fontFolder1 = @"C:\Windows\Fonts";
            string fontFolder2 = @"D:\CustomFonts";
            fontConfigs.SetFontFolder(fontFolder1, false);
            fontConfigs.SetFontFolder(fontFolder2, true);

            try
            {
                // Rufen Sie die aktuellen Schriftquellen ab.
                FontSourceBase[] fontSources = fontConfigs.GetFontSources();

                Console.WriteLine("Current font sources:");
                foreach (var source in fontSources)
                {
                    if (source is FolderFontSource folderSource)
                    {
                        Console.WriteLine($"- Folder: {folderSource.FolderPath} (Recursive: {folderSource.ScanSubFolders})");
                    }
                }

                // Erstelle eine Arbeitsmappe, um den Effekt zu demonstrieren
                Workbook workbook = new Workbook(FileFormatType.Xlsx);
                // Verwende die Schriftkonfigurationen beim Erstellen von Stilen oder beim Arbeiten mit Schriften
                // (Arbeitsbuch hat keine FontConfigs-Eigenschaft, daher entfernen wir diese Zeile)
                Worksheet worksheet = workbook.Worksheets[0];

                // Verwenden Sie eine benutzerdefinierte Schriftart, die sich möglicherweise in einem der Ordner befindet
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

### Siehe auch

* class [FontSourceBase](../../fontsourcebase/)
* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


