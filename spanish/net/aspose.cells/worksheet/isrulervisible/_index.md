---
title: "Worksheet.IsRulerVisible"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Worksheet property. Indica si la regla es visible. Esta propiedad solo se aplica en la vista previa de salto de página"
type: docs
url: /es/net/aspose.cells/worksheet/isrulervisible/
---
## Worksheet.IsRulerVisible property

Indica si la regla es visible. Esta propiedad solo se aplica en la vista previa de salto de página.

```csharp
public bool IsRulerVisible { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsRulerVisibleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer la hoja de cálculo a PageLayoutView donde la regla es visible
            worksheet.ViewType = ViewType.PageLayoutView;

            // Alternar la visibilidad de la regla
            worksheet.IsRulerVisible = true;

            // Mostrar el estado actual de visibilidad de la regla
            Console.WriteLine("Worksheet ruler is visible: " + worksheet.IsRulerVisible);

            // Guarda el libro de trabajo
            workbook.Save("WorksheetRulerVisibilityDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


