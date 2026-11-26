---
title: "ValidationCollection.RemoveACell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ValidationCollection. Elimina todas las configuraciones de validación en la celda"
type: docs
url: /es/net/aspose.cells/validationcollection/removeacell/
---
## ValidationCollection.RemoveACell method

Elimina todas las configuraciones de validación en la celda.

```csharp
public void RemoveACell(int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | El índice de fila de la celda. |
| columna | Int32 | El índice de columna de la celda. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationCollectionMethodRemoveACellWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar validación a la celda A1 (fila 0, columna 0)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            
            Validation validation = worksheet.Validations[worksheet.Validations.Add(area)];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Item1,Item2,Item3";

            // Eliminar validación de la celda A1
            worksheet.Validations.RemoveACell(0, 0);

            Console.WriteLine("Validations count after removal: " + worksheet.Validations.Count);
        }
    }
}
```

### Ver también

* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


