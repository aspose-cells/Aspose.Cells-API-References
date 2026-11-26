---
title: "IndividualFontConfigs.SetFontFolders"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método IndividualFontConfigs. Establece las carpetas de fuentes"
type: docs
url: /es/net/aspose.cells/individualfontconfigs/setfontfolders/
---
## IndividualFontConfigs.SetFontFolders method

Establece las carpetas de fuentes

```csharp
public void SetFontFolders(string[] fontFolders, bool recursive)
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

    public class IndividualFontConfigsMethodSetFontFoldersWithStringBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una instancia de IndividualFontConfigs
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Preparar la matriz de carpetas de fuentes
            string[] fontFolders = new string[] { @"C:\Windows\Fonts", @"D:\CustomFonts" };
            bool recursiveSearch = true;

            try
            {
                // Llame al método SetFontFolders con parámetros String[] y Boolean
                fontConfigs.SetFontFolders(fontFolders, recursiveSearch);

                // Demostrar el efecto usando una fuente personalizada
                worksheet.Cells["A1"].PutValue("Text with custom font");
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = "SomeCustomFont"; // Assuming this font exists in one of the folders
                worksheet.Cells["A1"].SetStyle(style);

                Console.WriteLine("SetFontFolders method executed successfully with parameters (String[], Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFontFolders method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("SetFontFoldersDemo.xlsx");
        }
    }
}
```

### Ver también

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


