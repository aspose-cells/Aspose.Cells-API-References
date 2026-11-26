---
title: "FontConfigs.GetFontFileDataInfo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FontConfigs. Obtén información de datos del archivo de fuente"
type: docs
url: /es/net/aspose.cells/fontconfigs/getfontfiledatainfo/
---
## FontConfigs.GetFontFileDataInfo method

Obtener información de datos del archivo de fuentes.

```csharp
public static FontFileDataInfo GetFontFileDataInfo(string fontName, bool isBold, bool isItalic, 
    bool isExactStyle)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fontName | String | nombre de fuente |
| isBold | Booleano | el estilo de la fuente es negrita o no |
| isItalic | Booleano | el estilo de la fuente es cursiva o no |
| isExactStyle | Booleano | si se debe coincidir exactamente con el estilo negrita/cursiva dado |

### Valor de retorno

Información de datos del archivo de fuente.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodGetFontFileDataInfoWithStringBooleanBooleanBooleanDemo
    {
        public static void Run()
        {
            try
            {
                // Llama a GetFontFileDataInfo con parámetros específicos (cambiado a llamada estática)
                FontFileDataInfo fontInfo = FontConfigs.GetFontFileDataInfo("Arial", true, false, false);

                // Mostrar información sobre los datos del archivo de fuente
                if (fontInfo != null)
                {
                    Console.WriteLine($"Font format type: {fontInfo.FormatType}");
                    Console.WriteLine($"Font data length: {fontInfo.Data?.Length ?? 0} bytes");
                }
                else
                {
                    Console.WriteLine("Font information not available");
                }

                // Demostrar el efecto en un libro de trabajo
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Establecer estilo con la fuente que verificamos
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.IsBold = true;
                style.Font.IsItalic = false;
                
                // Aplicar estilo a una celda
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].PutValue("Text with Arial Bold");

                // Guarda el libro de trabajo
                workbook.Save("FontConfigsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFontFileDataInfo method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [FontFileDataInfo](../../fontfiledatainfo/)
* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


