---
title: "HtmlSaveOptions.ParseHtmlTagInCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "HtmlSaveOptions propiedad. Indica si las etiquetas html, como div/div, en la celda deben analizarse como valor de celda o preservarse tal cual. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/parsehtmltagincell/
---
## HtmlSaveOptions.ParseHtmlTagInCell property

Indica si la etiqueta HTML (como `<div></div>`) en la celda debe analizarse como valor de celda o preservarse tal cual. El valor predeterminado es true.

```csharp
public bool ParseHtmlTagInCell { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyParseHtmlTagInCellDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo que contienen etiquetas HTML
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer el valor de la celda con etiquetas HTML
            worksheet.Cells["A1"].PutValue("<b>Bold Text</b> and <i>Italic Text</i>");
            
            // Crear opciones de guardado HTML y habilitar el análisis de etiquetas HTML
            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions(SaveFormat.Html);
            htmlSaveOptions.ParseHtmlTagInCell = true;
            
            // Guardar el libro de trabajo con etiquetas HTML analizadas
            workbook.Save("output.html", htmlSaveOptions);
            
            Console.WriteLine("HTML saved with ParseHtmlTagInCell enabled.");
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


