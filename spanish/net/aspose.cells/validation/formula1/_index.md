---
title: "Validation.Formula1"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de validación. Representa el valor o expresión asociado con la validación de datos"
type: docs
url: /es/net/aspose.cells/validation/formula1/
---
## Validation.Formula1 property

Representa el valor o expresión asociado a la validación de datos.

```csharp
public string Formula1 { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyFormula1Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar validación de lista con Formula1 como valores separados por comas
            Validation validation1 = worksheet.Validations[worksheet.Validations.Add()];
            validation1.Type = ValidationType.List;
            validation1.AlertStyle = ValidationAlertType.Stop;
            validation1.Formula1 = "A,B,C";
            validation1.AddArea(new CellArea() { StartRow = 0, StartColumn = 0, EndRow = 5, EndColumn = 0 });

            // Agregar validación de fórmula con Formula1 como referencia de celda
            Validation validation2 = worksheet.Validations[worksheet.Validations.Add()];
            validation2.Type = ValidationType.Custom;
            validation2.AlertStyle = ValidationAlertType.Stop;
            validation2.Formula1 = "=A5";
            validation2.AddArea(new CellArea() { StartRow = 0, StartColumn = 1, EndRow = 5, EndColumn = 1 });

            // Guardar y recargar para verificar la persistencia
            string outputPath = "output_validation_formula1.xlsx";
            workbook.Save(outputPath);

            // Recargar para verificar
            Workbook loadedWorkbook = new Workbook(outputPath);
            Worksheet loadedSheet = loadedWorkbook.Worksheets[0];

            Console.WriteLine("Validation 1 Formula1: " + loadedSheet.Validations[0].Formula1);
            Console.WriteLine("Validation 2 Formula1: " + loadedSheet.Validations[1].Formula1);
        }
    }
}
```

### Ver también

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


