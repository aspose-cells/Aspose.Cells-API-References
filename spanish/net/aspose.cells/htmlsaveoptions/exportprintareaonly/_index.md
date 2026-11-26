---
title: "HtmlSaveOptions.ExportPrintAreaOnly"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si solo se exporta el área de impresión al archivo html. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/exportprintareaonly/
---
## HtmlSaveOptions.ExportPrintAreaOnly property

Indica si solo se exporta el área de impresión al archivo html. El valor predeterminado es false.

```csharp
public bool ExportPrintAreaOnly { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportPrintAreaOnlyDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer datos de muestra
            for (int i = 0; i < 20; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i+1},{j+1}");
                }
            }

            // Establecer área de impresión
            worksheet.PageSetup.PrintArea = "B2:F10";

            // Configurar opciones de guardado HTML
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportPrintAreaOnly = true;
            options.ExportGridLines = true;

            // Guardar el libro de trabajo solo con el área de impresión
            workbook.Save("output.html", options);
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


