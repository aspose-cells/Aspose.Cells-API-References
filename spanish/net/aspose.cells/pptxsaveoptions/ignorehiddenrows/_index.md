---
title: "PptxSaveOptions.IgnoreHiddenRows"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PptxSaveOptions. Indica si se ignoran las filas ocultas al convertir Excel a PowerPoint"
type: docs
url: /es/net/aspose.cells/pptxsaveoptions/ignorehiddenrows/
---
## PptxSaveOptions.IgnoreHiddenRows property

Indica si se deben ignorar las filas ocultas al convertir Excel a PowerPoint.

```csharp
public bool IgnoreHiddenRows { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsPropertyIgnoreHiddenRowsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo y ocultar algunas filas
            worksheet.Cells["A1"].PutValue("Visible Row 1");
            worksheet.Cells["A2"].PutValue("Hidden Row");
            worksheet.Cells["A3"].PutValue("Visible Row 2");
            
            // Ocultar fila 2
            worksheet.Cells.Rows[1].IsHidden = true;

            // Establecer opciones de guardado PPTX con IgnoreHiddenRows
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.IgnoreHiddenRows = true;
            
            // Guardar como PPTX
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("PPTX saved with hidden rows ignored.");
        }
    }
}
```

### Ver también

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


