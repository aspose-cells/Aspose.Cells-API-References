---
title: "FontConfigs.SetFontSources"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FontConfigs. Imposta le font source"
type: docs
url: /it/net/aspose.cells/fontconfigs/setfontsources/
---
## FontConfigs.SetFontSources method

Imposta le fonti dei caratteri.

```csharp
public static void SetFontSources(FontSourceBase[] sources)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| origini | FontSourceBase[] | Un array di origini che contengono font TrueType. |

### Esempi

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
            // Crea un file di font temporaneo per dimostrazione
            string tempFontFile = Path.Combine(Path.GetTempPath(), "testfont.ttf");
            try
            {
                File.WriteAllBytes(tempFontFile, new byte[0]); // Empty file for demo

                // Crea font source
                FontSourceBase[] fontSources = new FontSourceBase[]
                {
                    new FolderFontSource(Path.GetTempPath(), true),
                    new FileFontSource(tempFontFile)
                };

                try
                {
                    // Chiama il metodo SetFontSources
                    FontConfigs.SetFontSources(fontSources);

                    // Verifica che le font source siano state impostate
                    FontSourceBase[] currentSources = FontConfigs.GetFontSources();
                    Console.WriteLine($"Font sources set successfully. Count: {currentSources.Length}");

                    // Dimostra l'effetto verificando se un font è disponibile
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
                // Pulisci
                if (File.Exists(tempFontFile))
                {
                    File.Delete(tempFontFile);
                }
            }
        }
    }
}
```

### Vedi anche

* class [FontSourceBase](../../fontsourcebase/)
* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


