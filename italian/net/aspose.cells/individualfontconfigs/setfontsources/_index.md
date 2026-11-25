---
title: "IndividualFontConfigs.SetFontSources"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo IndividualFontConfigs. Imposta le font sources"
type: docs
url: /it/net/aspose.cells/individualfontconfigs/setfontsources/
---
## IndividualFontConfigs.SetFontSources method

Imposta le fonti dei caratteri.

```csharp
public void SetFontSources(FontSourceBase[] sources)
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

    public class IndividualFontConfigsMethodSetFontSourcesWithFontSourceBaseDemo
    {
        public static void Run()
        {
            // Crea configurazioni di font individuali
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Prepara le font sources - usando sia la cartella che le font sources in memoria
            FontSourceBase[] fontSources = new FontSourceBase[]
            {
                new FolderFontSource(@"C:\Windows\Fonts", false),
                new MemoryFontSource(File.ReadAllBytes(@"C:\Windows\Fonts\arial.ttf"))
            };

            try
            {
                // Chiama SetFontSources con le font sources preparate
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

                // Crea una cartella di lavoro per dimostrare l'effetto
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Usa un font che dovrebbe essere disponibile dalle font sources
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].Value = "Text using font from custom sources";
                worksheet.Cells["A2"].Value = "This demonstrates SetFontSources with FontSourceBase[]";

                // Salva la cartella di lavoro
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

### Vedi anche

* class [FontSourceBase](../../fontsourcebase/)
* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


