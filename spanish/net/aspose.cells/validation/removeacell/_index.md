---
title: "Validation.RemoveACell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de validación. Elimina la configuración de validación en la celda"
type: docs
url: /es/net/aspose.cells/validation/removeacell/
---
## Validation.RemoveACell method

Elimine la configuración de validación en la celda.

```csharp
public void RemoveACell(int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | El índice de fila. |
| columna | Int32 | El índice de columna. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodRemoveACellWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar validación de datos a la primera celda
            Validation validation = worksheet.Validations[0];
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            validation.Type = ValidationType.List;
            validation.Formula1 = "1,2,3";
            
            // Agregar otra celda a la validación
            validation.AddArea(new CellArea { StartRow = 1, StartColumn = 1, EndRow = 1, EndColumn = 1 });
            
            // Eliminar la segunda celda de la validación
            validation.RemoveACell(1, 1);
            
            Console.WriteLine("Cell removed from validation successfully.");
        }
    }
}
```

### Ver también

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


