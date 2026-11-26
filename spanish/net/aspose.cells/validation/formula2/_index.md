---
title: "Validation.Formula2"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de validación. Representa el valor o expresión asociado con la validación de datos"
type: docs
url: /es/net/aspose.cells/validation/formula2/
---
## Validation.Formula2 property

Representa el valor o expresión asociado a la validación de datos.

```csharp
public string Formula2 { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyFormula2Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            sheet.Cells["B3"].PutValue(100);
            sheet.Cells["B7"].PutValue(50);
            
            // Crear validación para la celda B7
            Validation validation = sheet.Cells["B7"].GetValidation();
            
            // Establecer tipo de validación y fórmulas
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "=B3";  // Demonstrating Formula2 usage
            
            // Aplicar validación
            CellArea area = new CellArea();
            area.StartRow = 6;
            area.StartColumn = 1;
            area.EndRow = 6;
            area.EndColumn = 1;
            validation.AddArea(area);
            
            // Guarda el libro de trabajo
            workbook.Save("ValidationFormula2Demo.xlsx");
        }
    }
}
```

### Ver también

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


