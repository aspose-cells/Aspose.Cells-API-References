---
title: "PaginatedSaveOptions.AllColumnsInOnePagePerSheet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PaginatedSaveOptions. Si AllColumnsInOnePagePerSheet es true, todo el contenido de columnas de una hoja se exportará a una sola página en el resultado. El ancho del tamaño de papel de la configuración de página será ignorado y los demás ajustes de la configuración de página seguirán aplicándose"
type: docs
url: /es/net/aspose.cells/paginatedsaveoptions/allcolumnsinonepagepersheet/
---
## PaginatedSaveOptions.AllColumnsInOnePagePerSheet property

Si AllColumnsInOnePagePerSheet es verdadero, todo el contenido de columnas de una hoja se exportará a una sola página en el resultado. El ancho del tamaño de papel de la configuración de página será ignorado, y los demás ajustes de la configuración de página seguirán teniendo efecto.

```csharp
public bool AllColumnsInOnePagePerSheet { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyAllColumnsInOnePagePerSheetDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para demostrar el ajuste de columnas
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[0, i].PutValue("Column " + (i + 1));
                worksheet.Cells[1, i].PutValue("Sample data " + (i + 1));
            }

            // Crea opciones de guardado PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.OnePagePerSheet = true;
            pdfSaveOptions.AllColumnsInOnePagePerSheet = true;

            // Guardar el libro de trabajo con las opciones
            workbook.Save("output.pdf", pdfSaveOptions);

            Console.WriteLine("PDF saved with all columns in one page per sheet.");
        }
    }
}
```

### Ver también

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


