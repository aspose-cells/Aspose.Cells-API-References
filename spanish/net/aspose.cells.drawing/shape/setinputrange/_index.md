---
title: "Shape.SetInputRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Shape. Establece el rango utilizado para rellenar el control"
type: docs
url: /es/net/aspose.cells.drawing/shape/setinputrange/
---
## Shape.SetInputRange method

Establece el rango utilizado para rellenar el control.

```csharp
public void SetInputRange(string formula, bool isR1C1, bool isLocal)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fórmula | String | El rango utilizado para rellenar el control. |
| isR1C1 | Booleano | Si la fórmula necesita formatearse como R1C1. |
| isLocal | Booleano | Si la fórmula necesita formatearse según la configuración regional. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeMethodSetInputRangeWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crear un objeto libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra a las celdas A1:A10
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = i + 1;
            }

            // Agregar una forma de cuadro de lista
            Aspose.Cells.Drawing.Shape listBox = worksheet.Shapes.AddListBox(2, 0, 2, 0, 130, 130);

            // Establecer el rango de entrada para el cuadro de lista (usando parámetros String, Boolean, Boolean)
            listBox.SetInputRange("$A$1:$A$6", false, false);

            // Establecer la celda vinculada para el cuadro de lista
            listBox.SetLinkedCell("$A$12", false, true);

            // Guarda el libro de trabajo
            workbook.Save("SetInputRangeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


