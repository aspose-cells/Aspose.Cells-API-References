---
title: "Validation.Areas"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de validación. Obtiene todas las CellArea que contienen la configuración de validación de datos"
type: docs
url: /es/net/aspose.cells/validation/areas/
---
## Validation.Areas property

Obtiene todas las [`CellArea`](../../cellarea/) que contienen la configuración de validación de datos.

```csharp
public CellArea[] Areas { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyAreasDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets.Add("Areas & rent");

            // Crear validación para la columna A
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "1";
            validation.Formula2 = "100";

            // Agregar áreas de validación en diferentes filas
            validation.AddArea(new CellArea { StartRow = 46, StartColumn = 0, EndRow = 50, EndColumn = 0 });
            validation.AddArea(new CellArea { StartRow = 92, StartColumn = 0, EndRow = 96, EndColumn = 0 });
            validation.AddArea(new CellArea { StartRow = 138, StartColumn = 0, EndRow = 142, EndColumn = 0 });

            // Demostrar el acceso a áreas de validación
            CellArea area1 = (CellArea)validation.Areas[0];
            Console.WriteLine($"Area 1 StartRow: {area1.StartRow}"); // Output: 46
            
            CellArea area2 = (CellArea)validation.Areas[1];
            Console.WriteLine($"Area 2 StartRow: {area2.StartRow}"); // Output: 92
            
            CellArea area3 = (CellArea)validation.Areas[2];
            Console.WriteLine($"Area 3 StartRow: {area3.StartRow}"); // Output: 138
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


