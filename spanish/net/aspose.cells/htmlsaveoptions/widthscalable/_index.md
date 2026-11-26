---
title: "HtmlSaveOptions.WidthScalable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se exporta el ancho de columna en unidades de escala a HTML. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/widthscalable/
---
## HtmlSaveOptions.WidthScalable property

Indica si se exporta el ancho de columna en unidades de escala a HTML. El valor predeterminado es false.

```csharp
public bool WidthScalable { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyWidthScalableDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de muestra con datos de prueba
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test WidthScalable Property");
            worksheet.Cells["B1"].PutValue(123.45);
            
            // Establecer las opciones de guardado HTML con la propiedad WidthScalable
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.WidthScalable = true; // Demonstrate setting to true
            
            // Guardar con ancho escalable
            workbook.Save("output_scalable.html", options);
            
            // Guardar nuevamente con ancho fijo
            options.WidthScalable = false;
            workbook.Save("output_fixed.html", options);
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


