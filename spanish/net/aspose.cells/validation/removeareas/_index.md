---
title: "Validation.RemoveAreas"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de validación. Elimina esta validación de las áreas dadas"
type: docs
url: /es/net/aspose.cells/validation/removeareas/
---
## Validation.RemoveAreas method

Elimina esta validación de las áreas dadas.

```csharp
public void RemoveAreas(CellArea[] areas)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| áreas | CellArea[] | las áreas donde se deben eliminar estas configuraciones de validación. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodRemoveAreasWithCellAreaArrayDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar validación de datos a la hoja de cálculo
            int validationIndex = worksheet.Validations.Add();
            Validation validation = worksheet.Validations[validationIndex];
            
            // Configurar ajustes de validación
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "1";
            validation.Formula2 = "10";

            // Crear dos áreas de celdas para la validación
            CellArea area1 = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 1,
                EndColumn = 1
            };  // A1:B2
            CellArea area2 = new CellArea
            {
                StartRow = 2,
                StartColumn = 2,
                EndRow = 3,  // Original code had (2,2,1,1) which would be invalid endRow < startRow
                EndColumn = 3
            };  // C3:D4 (corrected end coordinates)
            
            // Agregar áreas a la validación
            validation.AddArea(area1);
            validation.AddArea(area2);
            Console.WriteLine($"Added areas: {validation.Areas.Length}");

            try
            {
                // Crear una matriz con una área para eliminar
                CellArea[] removeAreas = { area1 };
                
                // Ejecutar el método RemoveAreas
                validation.RemoveAreas(removeAreas);
                Console.WriteLine($"Remaining areas after removal: {validation.Areas.Length}");
                
                // Mostrar coordenadas de las áreas restantes
                foreach (CellArea remainingArea in validation.Areas)
                {
                    Console.WriteLine($"Area: {remainingArea.StartRow},{remainingArea.StartColumn} to {remainingArea.EndRow},{remainingArea.EndColumn}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Guardar el libro de trabajo modificado
            workbook.Save("ValidationRemoveAreasDemo.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


