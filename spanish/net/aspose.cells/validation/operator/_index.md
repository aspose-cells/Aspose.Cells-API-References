---
title: "Validation.Operator"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Validation. Representa el operador para la validación de datos"
type: docs
url: /es/net/aspose.cells/validation/operator/
---
## Validation.Operator property

Representa el operador de la validación de datos.

```csharp
public OperatorType Operator { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyOperatorDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la validación
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Crear un rango de validación
            CellArea area = CellArea.CreateCellArea("B1", "B5");
            int validationIndex = worksheet.Validations.Add(area);
            Validation validation = worksheet.Validations[validationIndex];

            // Establecer propiedades de validación con demostración de Operator
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "30";
            validation.ShowError = true;
            validation.ErrorMessage = "Value must be between 10 and 30";

            // Guarda el libro de trabajo
            workbook.Save("ValidationOperatorDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [OperatorType](../../operatortype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


