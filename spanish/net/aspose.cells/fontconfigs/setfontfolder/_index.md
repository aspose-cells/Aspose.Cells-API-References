---
title: "FontConfigs.SetFontFolder"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de FontConfigs. Establece la carpeta de fuentes"
type: docs
url: /es/net/aspose.cells/fontconfigs/setfontfolder/
---
## FontConfigs.SetFontFolder method

Establece la carpeta de fuentes

```csharp
public static void SetFontFolder(string fontFolder, bool recursive)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fontFolder | String | La carpeta que contiene fuentes TrueType. |
| recursivo | Booleano | Determina si escanear o no subcarpetas. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontConfigsMethodSetFontFolderWithStringBooleanDemo
    {
        public static void Run()
        {
            // Inicializa un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregue texto a la celda A1
            worksheet.Cells["A1"].PutValue("Sample Text with Custom Font");
            
            // Establezca la carpeta de fuentes personalizada y especifique si incluir subcarpetas
            FontConfigs.SetFontFolder("Fonts", true);
            
            // Aplique un estilo de fuente que pueda usar fuentes de la carpeta personalizada
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "CustomFont"; // Assuming "CustomFont" exists in the Fonts folder
            style.Font.Size = 14;
            worksheet.Cells["A1"].SetStyle(style);
            
            // Guarda el libro de trabajo en PDF
            workbook.Save("output.pdf", SaveFormat.Pdf);
        }
    }
}
```

### Ver también

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


