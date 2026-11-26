---
title: "Validation.InputTitle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Validation. Representa el título del cuadro de diálogo de entrada de validación de datos"
type: docs
url: /es/net/aspose.cells/validation/inputtitle/
---
## Validation.InputTitle property

Representa el título del cuadro de diálogo de entrada de validación de datos.

```csharp
public string InputTitle { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyInputTitleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un objeto de validación
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.IgnoreBlank = true;
            
            // Establecer el rango de validación
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 0;
            area.StartColumn = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            // Establezca propiedades de validación
            validation.Formula1 = "10";
            validation.Formula2 = "100";
            validation.Operator = OperatorType.Between;
            
            // Establecer las propiedades del mensaje de entrada
            validation.InputTitle = "Number Validation";
            validation.InputMessage = "Please enter a number between 10 and 100";
            
            // Guarda el libro de trabajo
            workbook.Save("ValidationInputTitleDemo.xlsx");
            
            // Verificar la propiedad InputTitle
            Console.WriteLine("Validation InputTitle: " + validation.InputTitle);
        }
    }
}
```

### Ver también

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


