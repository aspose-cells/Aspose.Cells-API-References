---
title: "IndividualFontConfigs.SetFontFolder"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método IndividualFontConfigs. Establece la carpeta de fuentes"
type: docs
url: /es/net/aspose.cells/individualfontconfigs/setfontfolder/
---
## IndividualFontConfigs.SetFontFolder method

Establece la carpeta de fuentes

```csharp
public void SetFontFolder(string fontFolder, bool recursive)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fontFolder | String | La carpeta que contiene fuentes TrueType. |
| recursivo | Booleano | Determina si escanear o no subcarpetas. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodSetFontFolderWithStringBooleanDemo
    {
        public static void Run()
        {
            // Crear una instancia de IndividualFontConfigs
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();
            
            // Especificar la ruta de la carpeta de fuentes y si se debe buscar recursivamente
            string fontFolderPath = @"C:\Windows\Fonts";
            bool recursiveSearch = true;

            try
            {
                // Llamar a SetFontFolder con los parámetros especificados
                fontConfigs.SetFontFolder(fontFolderPath, recursiveSearch);
                
                Console.WriteLine($"Successfully set font folder to: {fontFolderPath}");
                Console.WriteLine($"Recursive search enabled: {recursiveSearch}");

                // Crear un libro de trabajo para demostrar el uso de fuentes
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Establecer un estilo que podría usar fuentes de la carpeta especificada
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial"; // Assuming Arial exists in the font folder
                style.Font.Size = 12;
                
                worksheet.Cells["A1"].Value = "Text with font from specified folder";
                worksheet.Cells["A1"].SetStyle(style);
                
                // Guarda el libro de trabajo
                workbook.Save("FontConfigDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting font folder: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


