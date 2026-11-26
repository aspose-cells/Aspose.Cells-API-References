---
title: "HtmlSaveOptions.ExportBogusRowData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se exportan datos falsos de la fila inferior. El valor predeterminado es true. Si deseas importar el archivo html o mht a Excel, por favor mantén el valor predeterminado"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/exportbogusrowdata/
---
## HtmlSaveOptions.ExportBogusRowData property

Indica si se exportan datos falsos de la fila inferior. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado.

```csharp
public bool ExportBogusRowData { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportBogusRowDataDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos a las celdas
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // Crear opciones de guardado HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            
            // Primera exportación sin datos falsos de fila
            saveOptions.ExportBogusRowData = false;
            workbook.Save("output_without_bogus.html", saveOptions);
            
            // Luego exportar con datos falsos de fila
            saveOptions.ExportBogusRowData = true;
            workbook.Save("output_with_bogus.html", saveOptions);

            // Muestra los resultados
            Console.WriteLine("HTML files created successfully.");
            Console.WriteLine("Check output_without_bogus.html and output_with_bogus.html to see the difference.");
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


