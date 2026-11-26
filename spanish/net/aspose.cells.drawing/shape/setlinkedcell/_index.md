---
title: "Shape.SetLinkedCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Shape. Establece el rango vinculado al valor del control"
type: docs
url: /es/net/aspose.cells.drawing/shape/setlinkedcell/
---
## Shape.SetLinkedCell method

Establece el rango vinculado al valor del control.

```csharp
public void SetLinkedCell(string formula, bool isR1C1, bool isLocal)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fórmula | String | El rango vinculado al valor del control. |
| isR1C1 | Booleano | Si la fórmula necesita formatearse como R1C1. |
| isLocal | Booleano | Si la fórmula necesita formatearse según la configuración regional. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeMethodSetLinkedCellWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de barra de desplazamiento
            Aspose.Cells.Drawing.Shape scrollBar = worksheet.Shapes.AddScrollBar(2, 0, 2, 0, 130, 30);

            // Vincular el valor de la barra de desplazamiento a la celda A12
            scrollBar.SetLinkedCell("$A$12", false, true);

            // Guarda el libro de trabajo
            workbook.Save("SetLinkedCellDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


