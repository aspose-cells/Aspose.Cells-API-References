---
title: "Worksheet.Validations"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Obtiene la colección de configuraciones de validación de datos en la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/validations/
---
## Worksheet.Validations property

Obtiene la colección de configuraciones de validación de datos en la hoja de cálculo.

```csharp
public ValidationCollection Validations { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyValidationsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar validación de datos a la celda A1
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Option1,Option2,Option3";
            
            // Corrección: Crear CellArea con StartRow, StartColumn, EndRow, EndColumn
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            // Obtener validación de la celda A1
            Validation cellValidation = worksheet.Validations.GetValidationInCell(0, 0);
            
            // Mostrar tipo de validación
            Console.WriteLine("Validation type in A1: " + cellValidation.Type);
            
            // Guarda el libro de trabajo
            workbook.Save("ValidationDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ValidationCollection](../../validationcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


