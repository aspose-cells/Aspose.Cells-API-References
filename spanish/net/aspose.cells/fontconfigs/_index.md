---
title: "Clase FontConfigs"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.FontConfigs. Especifica la configuración de fuentes"
type: docs
url: /es/net/aspose.cells/fontconfigs/
---
## FontConfigs class

Especifica la configuración de fuentes

```csharp
public class FontConfigs
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [FontConfigs](fontconfigs/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| static [DefaultFontName](../../aspose.cells/fontconfigs/defaultfontname/) { get; set; } | Obtiene o establece el nombre de fuente predeterminado. |
| static [PreferSystemFontSubstitutes](../../aspose.cells/fontconfigs/prefersystemfontsubstitutes/) { get; set; } | Indique si se deben usar sustitutos de fuentes del sistema primero o no cuando una fuente no está presente y el sustituto de esa fuente no está configurado. Por ejemplo, en Ubuntu, la fuente "Arial" suele ser sustituida por "Liberation Sans". El valor predeterminado es false. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [GetFontFileDataInfo](../../aspose.cells/fontconfigs/getfontfiledatainfo/)(string, bool, bool, bool) | Obtener información de datos del archivo de fuentes. |
| static [GetFontSources](../../aspose.cells/fontconfigs/getfontsources/)() | Obtiene una copia del arreglo que contiene la lista de fuentes |
| static [GetFontSubstitutes](../../aspose.cells/fontconfigs/getfontsubstitutes/)(string) | Devuelve un arreglo que contiene nombres de sustitutos de fuentes para usar si la fuente original no está presente. |
| static [IsFontAvailable](../../aspose.cells/fontconfigs/isfontavailable/)(string) | Indique si la fuente está disponible. |
| static [SetFontFolder](../../aspose.cells/fontconfigs/setfontfolder/)(string, bool) | Establece la carpeta de fuentes |
| static [SetFontFolders](../../aspose.cells/fontconfigs/setfontfolders/)(string[], bool) | Establece la carpeta de fuentes |
| static [SetFontSources](../../aspose.cells/fontconfigs/setfontsources/)(FontSourceBase[]) | Establece las fuentes de tipografía. |
| static [SetFontSubstitutes](../../aspose.cells/fontconfigs/setfontsubstitutes/)(string, string[]) | Nombres de sustitutos de fuentes para el nombre de fuente original dado. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFontConfigsDemo
    {
        public static void Run()
        {
            // Establecer carpeta de fuentes personalizada
            string fontFolder = @"C:\MyFonts\";
            FontConfigs.SetFontFolder(fontFolder, true);

            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer texto de muestra con diferentes fuentes
            worksheet.Cells["A1"].PutValue("Text with default font");
            worksheet.Cells["A2"].PutValue("Text with custom font");
            
            // Aplicar estilo de fuente personalizado
            Style style = workbook.CreateStyle();
            style.Font.Name = "MyCustomFont"; // This font should exist in the custom font folder
            worksheet.Cells["A2"].SetStyle(style);

            // Guardar a HTML para demostrar la renderización de fuentes
            HtmlSaveOptions options = new HtmlSaveOptions
            {
                ExportImagesAsBase64 = true,
                PresentationPreference = true
            };
            
            workbook.Save("output.html", options);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


