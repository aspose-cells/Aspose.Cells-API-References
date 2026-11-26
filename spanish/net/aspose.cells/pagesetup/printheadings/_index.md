---
title: "PageSetup.PrintHeadings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Representa si los encabezados de filas y columnas se imprimen en esta página"
type: docs
url: /es/net/aspose.cells/pagesetup/printheadings/
---
## PageSetup.PrintHeadings property

Representa si los encabezados de filas y columnas se imprimen con esta página.

```csharp
public bool PrintHeadings { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintHeadingsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer algunos datos de ejemplo con encabezados
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);

            // Habilitar la impresión de encabezados
            worksheet.PageSetup.PrintHeadings = true;
            worksheet.PageSetup.PrintArea = "A1:B3";

            // Guardar como HTML para demostrar el efecto
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportActiveWorksheetOnly = true,
                ExportPrintAreaOnly = true,
                ExportGridLines = true,
                ExportHeadings = true
            };

            workbook.Save("PrintHeadingsDemo.html", saveOptions);

            Console.WriteLine("Worksheet saved with PrintHeadings enabled.");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


