---
title: "FontConfigs.SetFontFolders"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de FontConfigs. Establece la carpeta de fuentes"
type: docs
url: /es/net/aspose.cells/fontconfigs/setfontfolders/
---
## FontConfigs.SetFontFolders method

Establece la carpeta de fuentes

```csharp
public static void SetFontFolders(string[] fontFolders, bool recursive)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fontFolders | String[] | Las carpetas que contienen fuentes TrueType. |
| recursivo | Booleano | Determina si escanear o no subcarpetas. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodSetFontFoldersWithStringBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establezca texto que utilizará fuentes personalizadas
            worksheet.Cells["A1"].PutValue("Text with custom font");

            // Prepare carpetas de fuentes (reemplace con rutas reales en su sistema)
            string[] fontFolders = new string[] 
            {
                @"C:\Windows\Fonts",
                @"D:\CustomFonts"
            };
            bool recursiveSearch = true;

            try
            {
                // Llame al método SetFontFolders con parámetros String[] y Boolean
                FontConfigs.SetFontFolders(fontFolders, recursiveSearch);

                // Aplique una fuente que pueda estar en una de estas carpetas
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = "SomeCustomFont"; // Replace with actual font name
                worksheet.Cells["A1"].SetStyle(style);

                Console.WriteLine("Font folders set successfully. Workbook may use fonts from these locations.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting font folders: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("FontConfigsSetFontFoldersDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


