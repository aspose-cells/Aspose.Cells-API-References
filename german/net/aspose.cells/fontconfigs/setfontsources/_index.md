---
title: "FontConfigs.SetFontSources"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FontConfigs-Methode. Legt die Schriftquellen fest"
type: docs
url: /de/net/aspose.cells/fontconfigs/setfontsources/
---
## FontConfigs.SetFontSources method

Legt die Schriftquellen fest.

```csharp
public static void SetFontSources(FontSourceBase[] sources)
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

    public class FontConfigsMethodSetFontSourcesWithFontSourceBaseDemo
    {
        public static void Run()
        {
            // Erstelle eine temporäre Schriftdatei zum Demonstrieren
            string tempFontFile = Path.Combine(Path.GetTempPath(), "testfont.ttf");
            try
            {
                File.WriteAllBytes(tempFontFile, new byte[0]); // Empty file for demo

                // Schriftquellen erstellen
                FontSourceBase[] fontSources = new FontSourceBase[]
                {
                    new FolderFontSource(Path.GetTempPath(), true),
                    new FileFontSource(tempFontFile)
                };

                try
                {
                    // Rufe die SetFontSources-Methode auf
                    FontConfigs.SetFontSources(fontSources);

                    // Überprüfe, ob die Schriftquellen gesetzt wurden
                    FontSourceBase[] currentSources = FontConfigs.GetFontSources();
                    Console.WriteLine($"Font sources set successfully. Count: {currentSources.Length}");

                    // Demonstriere die Wirkung, indem geprüft wird, ob eine Schrift verfügbar ist
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
                // Aufräumen
                if (File.Exists(tempFontFile))
                {
                    File.Delete(tempFontFile);
                }
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


