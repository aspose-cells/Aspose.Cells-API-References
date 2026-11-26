---
title: "IndividualFontConfigs.GetFontSources"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método IndividualFontConfigs. Obtiene una copia de la matriz que contiene la lista de fuentes"
type: docs
url: /es/net/aspose.cells/individualfontconfigs/getfontsources/
---
## IndividualFontConfigs.GetFontSources method

Obtiene una copia del arreglo que contiene la lista de fuentes

```csharp
public FontSourceBase[] GetFontSources()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodGetFontSourcesDemo
    {
        public static void Run()
        {
            // Crear configuraciones de fuentes individuales
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Establecer algunos orígenes de fuentes (carpetas que contienen fuentes)
            string fontFolder1 = @"C:\Windows\Fonts";
            string fontFolder2 = @"D:\CustomFonts";
            fontConfigs.SetFontFolder(fontFolder1, false);
            fontConfigs.SetFontFolder(fontFolder2, true);

            try
            {
                // Obtenga los orígenes de fuentes actuales
                FontSourceBase[] fontSources = fontConfigs.GetFontSources();

                Console.WriteLine("Current font sources:");
                foreach (var source in fontSources)
                {
                    if (source is FolderFontSource folderSource)
                    {
                        Console.WriteLine($"- Folder: {folderSource.FolderPath} (Recursive: {folderSource.ScanSubFolders})");
                    }
                }

                // Crear un libro de trabajo para demostrar el efecto
                Workbook workbook = new Workbook(FileFormatType.Xlsx);
                // Usar las configuraciones de fuentes al crear estilos o trabajar con fuentes
                // (Workbook no tiene una propiedad FontConfigs, así que eliminamos esa línea)
                Worksheet worksheet = workbook.Worksheets[0];

                // Usar una fuente personalizada que podría estar en una de las carpetas
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

### Ver también

* class [FontSourceBase](../../fontsourcebase/)
* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


