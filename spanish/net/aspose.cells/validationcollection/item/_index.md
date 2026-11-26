---
title: "ValidationCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ValidationCollection. Obtiene el elemento Validation en el índice especificado"
type: docs
url: /es/net/aspose.cells/validationcollection/item/
---
## ValidationCollection indexer

Obtiene el elemento [`Validation`](../../validation/) en el índice especificado.

```csharp
public Validation this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice basado en cero del elemento. |

### Valor de retorno

El elemento en el índice especificado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar validación de datos a las celdas
            ValidationCollection validations = sheet.Validations;
            
            // Primera área de validación
            Validation validation1 = validations[validations.Add()];
            validation1.AddArea(new CellArea { StartRow = 1, StartColumn = 1, EndRow = 4, EndColumn = 3 });
            
            // Segunda área de validación
            Validation validation2 = validations[validations.Add()];
            validation2.AddArea(new CellArea { StartRow = 6, StartColumn = 1, EndRow = 6, EndColumn = 3 });

            // Acceder a la validación usando la propiedad Item
            Validation firstValidation = validations[0];
            Console.WriteLine($"First validation has {firstValidation.Areas.Length} area(s)");

            // Verificar áreas
            foreach (CellArea area in firstValidation.Areas)
            {
                Console.WriteLine($"Area: {area.StartRow},{area.StartColumn} to {area.EndRow},{area.EndColumn}");
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


