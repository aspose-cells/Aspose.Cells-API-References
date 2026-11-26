---
title: "Validation.RemoveArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de validación. Elimina la configuración de validación en el rango"
type: docs
url: /es/net/aspose.cells/validation/removearea/
---
## Validation.RemoveArea method

Elimine la configuración de validación en el rango.

```csharp
public void RemoveArea(CellArea cellArea)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellArea | CellArea | las áreas donde se deben eliminar estas configuraciones de validación. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodRemoveAreaWithCellAreaDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una validación a la hoja de cálculo
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "100";

            // Agregar área de validación inicial
            CellArea initialArea = CellArea.CreateCellArea(0, 0, 0, 0);
            validation.AddArea(initialArea);

            // Agregar otra área a la validación
            CellArea additionalArea = CellArea.CreateCellArea(1, 1, 1, 1);
            validation.AddArea(additionalArea);

            Console.WriteLine("Validation areas count after adding: " + validation.Areas.Length);

            // Eliminar el área adicional
            validation.RemoveArea(additionalArea);

            Console.WriteLine("Validation areas count after removing: " + validation.Areas.Length);

            // Agregar múltiples áreas
            CellArea[] multipleAreas = new CellArea[]
            {
                CellArea.CreateCellArea(2, 2, 2, 2),
                CellArea.CreateCellArea(3, 3, 3, 3),
                CellArea.CreateCellArea(4, 4, 4, 4)
            };
            validation.AddAreas(multipleAreas, false, false);

            Console.WriteLine("Validation areas count after adding multiple: " + validation.Areas.Length);

            // Eliminar una de las áreas
            validation.RemoveArea(multipleAreas[1]);

            Console.WriteLine("Validation areas count after removing one: " + validation.Areas.Length);
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


