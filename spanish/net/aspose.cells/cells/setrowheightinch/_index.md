---
title: "Cells.SetRowHeightInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Establece la altura de la fila en unidades de pulgadas"
type: docs
url: /es/net/aspose.cells/cells/setrowheightinch/
---
## Cells.SetRowHeightInch method

Establece la altura de la fila en unidades de pulgadas.

```csharp
public void SetRowHeightInch(int row, double inches)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila. |
| pulgadas | Double | Número de pulgadas. Debe estar entre 0 y 409.5/72. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetRowHeightInchWithInt32DoubleDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer estilo predeterminado
            Style style = workbook.DefaultStyle;
            style.Font.Name = "Tahoma";
            style.Font.Size = 16;
            style.Font.IsBold = true;
            workbook.DefaultStyle = style;

            // Establecer alturas de fila en pulgadas
            for (int i = 0; i < 10; i++)
            {
                cells.SetRowHeightInch(i, 0.5 + (i * 0.2)); // Demonstrates SetRowHeightInch(Int32, Double)
            }

            // Guarda el libro de trabajo
            workbook.Save("RowHeightsInInches.xlsx");
            
            Console.WriteLine("Row heights set successfully in inches.");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


