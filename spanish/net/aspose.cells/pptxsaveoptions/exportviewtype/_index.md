---
title: "PptxSaveOptions.ExportViewType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PptxSaveOptions. Obtiene y establece el tipo de visualización al exportar a PowerPoint. El tipo de exportación predeterminado funciona como impresión"
type: docs
url: /es/net/aspose.cells/pptxsaveoptions/exportviewtype/
---
## PptxSaveOptions.ExportViewType property

Obtiene y establece el tipo de visualización al exportar a PowerPoint. El tipo de exportación predeterminado funciona como impresión.

```csharp
public SlideViewType ExportViewType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsPropertyExportViewTypeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Establecer opciones de guardado PPTX con ExportViewType
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.ExportViewType = SlideViewType.View;
            
            // Guardar el libro de trabajo como PPTX
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("Workbook saved as PPTX with ExportViewType set to View");
        }
    }
}
```

### Ver también

* enum [SlideViewType](../../../aspose.cells.slides/slideviewtype/)
* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


