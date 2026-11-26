---
title: "FontConfigs.GetFontSources"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de FontConfigs. Obtiene una copia del arreglo que contiene la lista de orígenes"
type: docs
url: /es/net/aspose.cells/fontconfigs/getfontsources/
---
## FontConfigs.GetFontSources method

Obtiene una copia del arreglo que contiene la lista de fuentes

```csharp
public static FontSourceBase[] GetFontSources()
```

### Ejemplos

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
                // Obtenga los orígenes de fuentes actuales
                FontSourceBase[] fontSources = FontConfigs.GetFontSources();

                // Muestre información sobre cada origen de fuente
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

                // Crea un nuevo libro de trabajo para demostrar el efecto
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Establece algún texto con una fuente que podría usar estos recursos
                worksheet.Cells["A1"].PutValue("Font Sources Demo");
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                worksheet.Cells["A1"].SetStyle(style);

                // Guarda el libro de trabajo
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

### Ver también

* class [FontSourceBase](../../fontsourcebase/)
* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


