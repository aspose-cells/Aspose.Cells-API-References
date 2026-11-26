---
title: "HtmlSaveOptions.ExportRowColumnHeadings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se exportan los encabezados de filas y columnas de las hojas al guardar en archivos HTML"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/exportrowcolumnheadings/
---
## HtmlSaveOptions.ExportRowColumnHeadings property

Indica si se exportan los encabezados de filas y columnas de la hoja al guardar en archivos HTML.

```csharp
public bool ExportRowColumnHeadings { get; set; }
```

### Observaciones

El valor predeterminado es false.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportRowColumnHeadingsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);

            // Crear opciones de guardado HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Establecer ExportRowColumnHeadings en false (el valor predeterminado es true)
            saveOptions.ExportRowColumnHeadings = false;

            // Guardar el libro de trabajo con los encabezados desactivados
            workbook.Save("output_without_headings.html", saveOptions);

            // Ahora habilita los encabezados y guarda de nuevo
            saveOptions.ExportRowColumnHeadings = true;
            workbook.Save("output_with_headings.html", saveOptions);

            Console.WriteLine("HTML files saved with different heading visibility settings.");
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


