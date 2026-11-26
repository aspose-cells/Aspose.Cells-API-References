---
title: "Range.ToHtml"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Convertir el rango a HTML"
type: docs
url: /es/net/aspose.cells/range/tohtml/
---
## Range.ToHtml method

Convertir el rango a html.

```csharp
public byte[] ToHtml(HtmlSaveOptions saveOptions)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| saveOptions | HtmlSaveOptions | Opciones para convertir el rango a HTML. |

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodToHtmlWithHtmlSaveOptionsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Poblar algunos datos en el rango A1:J25
            for (int i = 0; i < 25; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].Value = $"Cell {i+1},{j+1}";
                }
            }

            // Crear un rango con el nombre de tipo totalmente calificado
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:J25");
            
            // Crear opciones de guardado HTML
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportImagesAsBase64 = true;
            
            // Convertir el rango a HTML
            byte[] htmlData = range.ToHtml(options);
            
            // Guardar HTML en un archivo
            File.WriteAllBytes("output.html", htmlData);
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../../htmlsaveoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


