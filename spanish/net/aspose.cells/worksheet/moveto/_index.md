---
title: "Worksheet.MoveTo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Worksheet method. Mueve la hoja a otra ubicación en la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/moveto/
---
## Worksheet.MoveTo method

Mueve la hoja a otra ubicación en la hoja de cálculo.

```csharp
public void MoveTo(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | Índice de hoja de destino. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodMoveToWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar algunas hojas de cálculo
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Agregar una nueva hoja de cálculo y moverla a la posición 1
            Worksheet newWorksheet = workbook.Worksheets.Add("MovedSheet");
            newWorksheet.MoveTo(1);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


