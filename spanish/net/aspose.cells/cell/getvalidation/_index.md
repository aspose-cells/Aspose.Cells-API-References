---
title: "Cell.GetValidation"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Obtiene la validación aplicada a esta celda"
type: docs
url: /es/net/aspose.cells/cell/getvalidation/
---
## Cell.GetValidation method

Obtiene la validación aplicada a esta celda.

```csharp
public Validation GetValidation()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetValidationDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accede a la celda B5 y agrega validación
            Cell cell = worksheet.Cells["B5"];
            Validation validation = cell.GetValidation();
            
            // Establece el tipo de validación y muestra el mensaje
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";
            validation.ShowError = true;
            validation.ErrorMessage = "Enter value between 10 and 20";
            
            // Guarda el libro de trabajo
            workbook.Save("ValidationDemo.xlsx");
            
            // Verifica la validación
            Validation retrievedValidation = cell.GetValidation();
            Console.WriteLine("Validation Type: " + retrievedValidation.Type);
            Console.WriteLine("Validation Message: " + retrievedValidation.ErrorMessage);
        }
    }
}
```

### Ver también

* class [Validation](../../validation/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


