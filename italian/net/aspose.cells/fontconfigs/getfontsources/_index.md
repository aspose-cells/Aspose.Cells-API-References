---
title: "FontConfigs.GetFontSources"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FontConfigs. Ottiene una copia dell'array che contiene l'elenco delle font source"
type: docs
url: /it/net/aspose.cells/fontconfigs/getfontsources/
---
## FontConfigs.GetFontSources method

Ottiene una copia dell'array che contiene l'elenco delle fonti.

```csharp
public static FontSourceBase[] GetFontSources()
```

### Esempi

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
                // Ottieni le font source attuali
                FontSourceBase[] fontSources = FontConfigs.GetFontSources();

                // Visualizza le informazioni su ogni font source
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

                // Crea un nuovo workbook per dimostrare l'effetto
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Imposta del testo con un font che potrebbe utilizzare queste risorse
                worksheet.Cells["A1"].PutValue("Font Sources Demo");
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                worksheet.Cells["A1"].SetStyle(style);

                // Salva la cartella di lavoro
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

### Vedi anche

* class [FontSourceBase](../../fontsourcebase/)
* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


