---
title: "Style.IsTextWrapped"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Obtiene o establece un valor que indica si el texto dentro de una celda está envuelto"
type: docs
url: /es/net/aspose.cells/style/istextwrapped/
---
## Style.IsTextWrapped property

Obtiene o establece un valor que indica si el texto dentro de una celda está ajustado.

```csharp
public bool IsTextWrapped { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsTextWrappedDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            Cells cells = ws.Cells;
            
            // Establecer texto largo en la celda
            Cell cell = cells["A1"];
            cell.PutValue("This is a long text that should be wrapped in the cell");
            
            // Habilitar el ajuste de texto
            Style style = cell.GetStyle();
            style.IsTextWrapped = true;
            cell.SetStyle(style);
            
            // Ajustar la altura de la fila para mostrar el texto envuelto
            ws.AutoFitRow(0);
            
            // Guarda el libro de trabajo
            wb.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


