---
title: "Worksheet.GetPanes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Worksheet método. Obtiene los paneles de la ventana"
type: docs
url: /es/net/aspose.cells/worksheet/getpanes/
---
## Worksheet.GetPanes method

Obtiene los paneles de la ventana.

```csharp
public PaneCollection GetPanes()
```

### Observaciones

Si la ventana no está dividida o congelada.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetPanesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Congela los paneles en la fila 5 y la columna 3
            worksheet.FreezePanes(5, 3, 5, 3);
            
            // Obtener información del panel
            PaneCollection panes = worksheet.GetPanes();
            
            // Mostrar información del panel
            Console.WriteLine("First visible row of bottom pane: " + panes.FirstVisibleRowOfBottomPane);
            Console.WriteLine("First visible column of right pane: " + panes.FirstVisibleColumnOfRightPane);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [PaneCollection](../../panecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


