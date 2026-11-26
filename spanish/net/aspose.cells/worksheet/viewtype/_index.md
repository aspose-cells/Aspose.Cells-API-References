---
title: "Worksheet.ViewType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Obtiene y establece el tipo de vista"
type: docs
url: /es/net/aspose.cells/worksheet/viewtype/
---
## Worksheet.ViewType property

Obtiene y establece el tipo de vista.

```csharp
public ViewType ViewType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyViewTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establece el tipo de vista a PageLayoutView y habilita la regla
            worksheet.ViewType = ViewType.PageLayoutView;
            worksheet.IsRulerVisible = true;
            
            // Agrega contenido de muestra para demostrar la vista
            worksheet.Cells["A1"].PutValue("Page Layout View Demo");
            worksheet.Cells["A2"].PutValue("Ruler is visible in this view");
            
            // Guarda el libro de trabajo
            workbook.Save("WorksheetViewTypeDemo.xlsx");
            
            Console.WriteLine("Worksheet ViewType demo completed successfully.");
        }
    }
}
```

### Ver también

* enum [ViewType](../../viewtype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


