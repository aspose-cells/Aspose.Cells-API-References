---
title: "HtmlSaveOptions.AddTooltipText"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se agrega texto de información sobre herramientas cuando los datos no pueden mostrarse completamente. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/addtooltiptext/
---
## HtmlSaveOptions.AddTooltipText property

Indica si se agrega texto de información sobre herramientas cuando los datos no pueden mostrarse completamente. El valor predeterminado es false.

```csharp
public bool AddTooltipText { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyAddTooltipTextDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer un texto largo que exceda el ancho de la celda
            worksheet.Cells["A1"].PutValue("This is a long text that will exceed cell width and need tooltip");
            worksheet.Cells.SetColumnWidth(0, 10); // Set narrow column width
            
            // Configurar las opciones de guardado HTML con información sobre herramientas
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.AddTooltipText = true;
            
            // Guarda el libro de trabajo
            string outputPath = "output_with_tooltip.html";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("File saved with tooltips: " + outputPath);
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


