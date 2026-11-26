---
title: "Worksheet.PaneState"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Indica si el panel tiene divisiones horizontales o verticales y si esas divisiones están congeladas"
type: docs
url: /es/net/aspose.cells/worksheet/panestate/
---
## Worksheet.PaneState property

Indica si el panel tiene divisiones horizontales o verticales, y si esas divisiones están congeladas.

```csharp
public PaneStateType PaneState { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyPaneStateDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer datos de muestra
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");

            // Congelar paneles (primera fila)
            worksheet.FreezePanes(1, 0, 1, 0);

            // Obtener y mostrar el estado del panel
            PaneStateType paneState = worksheet.PaneState;
            Console.WriteLine("Pane State: " + paneState);

            // Guardar el libro de trabajo
            workbook.Save("PaneStateDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PaneStateType](../../panestatetype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


