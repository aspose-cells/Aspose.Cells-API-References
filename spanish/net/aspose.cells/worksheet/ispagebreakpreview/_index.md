---
title: "Worksheet.IsPageBreakPreview"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Worksheet. Indica si la hoja de cálculo especificada se muestra en vista normal o vista previa de salto de página"
type: docs
url: /es/net/aspose.cells/worksheet/ispagebreakpreview/
---
## Worksheet.IsPageBreakPreview property

Indica si la hoja de cálculo especificada se muestra en vista normal o vista previa de salto de página.

```csharp
public bool IsPageBreakPreview { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsPageBreakPreviewDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establezca la hoja de cálculo en modo Vista previa de salto de página
            worksheet.IsPageBreakPreview = true;
            
            // Establezca el zoom al 100 % para la demostración
            worksheet.Zoom = 100;
            
            // Muestre la configuración actual
            Console.WriteLine("IsPageBreakPreview: " + worksheet.IsPageBreakPreview);
            Console.WriteLine("Zoom: " + worksheet.Zoom);
            
            // Guarda el libro de trabajo
            workbook.Save("WorksheetPropertyIsPageBreakPreviewDemo_output.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


