---
title: "HtmlSaveOptions.DefaultFontName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Especifica el nombre de fuente predeterminado para exportar html; la fuente predeterminada se usará cuando la fuente del estilo no exista. Si esta propiedad es null, Aspose.Cells usará una fuente universal que tenga la misma familia que la fuente original. El valor predeterminado es null."
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/defaultfontname/
---
## HtmlSaveOptions.DefaultFontName property

Especifique el nombre de fuente predeterminado para exportar html; la fuente predeterminada se usará cuando la fuente del estilo no exista. Si esta propiedad es null, Aspose.Cells utilizará una fuente universal que tenga la misma familia que la fuente original. El valor predeterminado es null.

```csharp
public string DefaultFontName { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyDefaultFontNameDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Sample Text");
            
            // Establecer opciones de guardado HTML con fuente predeterminada personalizada
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.DefaultFontName = "Courier New";
            
            // Guardar a HTML con la fuente especificada
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML file saved with default font: " + saveOptions.DefaultFontName);
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


