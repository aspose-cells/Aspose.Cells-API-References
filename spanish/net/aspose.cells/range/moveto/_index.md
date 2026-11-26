---
title: "Range.MoveTo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Mueve el rango actual al rango de destino"
type: docs
url: /es/net/aspose.cells/range/moveto/
---
## Range.MoveTo method

Mueve el rango actual al rango de destino.

```csharp
public void MoveTo(int destRow, int destColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destRow | Int32 | La fila inicial del rango de destino. |
| destColumn | Int32 | La columna inicial del rango de destino. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodMoveToWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un rango de ejemplo (A1:B2)
            Aspose.Cells.Range originalRange = worksheet.Cells.CreateRange("A1", "B2");
            
            // Coloca algunos datos en el rango para demostración
            originalRange[0, 0].PutValue("A1");
            originalRange[0, 1].PutValue("B1");
            originalRange[1, 0].PutValue("A2");
            originalRange[1, 1].PutValue("B2");
            
            // Mueve el rango hacia abajo 1 fila (a A2:B3)
            originalRange.MoveTo(originalRange.FirstRow + 1, originalRange.FirstColumn);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


