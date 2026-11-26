---
title: "IndividualFontConfigs.SetFontSources"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método IndividualFontConfigs. Establece las fuentes tipográficas"
type: docs
url: /es/net/aspose.cells/individualfontconfigs/setfontsources/
---
## IndividualFontConfigs.SetFontSources method

Establece las fuentes de tipografía.

```csharp
public void SetFontSources(FontSourceBase[] sources)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| orígenes | FontSourceBase[] | Una matriz de orígenes que contienen fuentes TrueType. |

### Ejemplos

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
            // Crear configuraciones de fuentes individuales
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Preparar fuentes tipográficas - usando tanto fuentes de carpeta como fuentes de memoria
            FontSourceBase[] fontSources = new FontSourceBase[]
            {
                new FolderFontSource(@"C:\Windows\Fonts", false),
                new MemoryFontSource(File.ReadAllBytes(@"C:\Windows\Fonts\arial.ttf"))
            };

            try
            {
                // Llamar a SetFontSources con las fuentes tipográficas preparadas
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

                // Crear un libro de trabajo para demostrar el efecto
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Usar una fuente que debería estar disponible en las fuentes
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].Value = "Text using font from custom sources";
                worksheet.Cells["A2"].Value = "This demonstrates SetFontSources with FontSourceBase[]";

                // Guarda el libro de trabajo
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

### Ver también

* class [FontSourceBase](../../fontsourcebase/)
* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


