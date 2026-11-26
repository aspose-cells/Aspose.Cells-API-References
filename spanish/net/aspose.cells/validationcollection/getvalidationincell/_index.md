---
title: "ValidationCollection.GetValidationInCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ValidationCollection. Obtiene la validación aplicada a la celda dada"
type: docs
url: /es/net/aspose.cells/validationcollection/getvalidationincell/
---
## ValidationCollection.GetValidationInCell method

Obtiene la validación aplicada a la celda dada.

```csharp
public Validation GetValidationInCell(int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | El índice de fila. |
| columna | Int32 | El índice de columna. |

### Valor de retorno

Devuelve un objeto [`Validation`](../../validation/) o null si no hay validación para la celda dada

### Ejemplos

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationCollectionMethodGetValidationInCellWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar validación de datos a la celda A1 (0,0)
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.List;
            validation.Formula1 = "\"Option1,Option2,Option3\"";
            
            // Crear CellArea con StartRow, StartColumn, EndRow, EndColumn
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            // Obtener validación de la celda A1 (0,0)
            Validation validationInCell = worksheet.Validations.GetValidationInCell(0, 0);
            
            if (validationInCell != null && validationInCell.Type == ValidationType.List)
            {
                Console.WriteLine("Cell A1 has list validation with formula: " + validationInCell.Formula1);
            }
        }
    }
}
```

### Ver también

* class [Validation](../../validation/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


