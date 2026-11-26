---
title: "Validation.Value1"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Validation. Representa el primer valor asociado a la validación de datos"
type: docs
url: /es/net/aspose.cells/validation/value1/
---
## Validation.Value1 property

Representa el primer valor asociado a la validación de datos.

```csharp
public object Value1 { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyValue1Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una validación en la celda A1
            Validation validation = worksheet.Cells["A1"].GetValidation();
            validation.Type = ValidationType.List;
            
            // Establece la propiedad Value1 con una matriz de cadenas
            validation.Value1 = new object[] { "Option1", "Option2", "Option3" };

            // Obtén y muestra los valores de la validación
            object[] values = validation.Value1 as object[];
            Console.WriteLine("Validation values in A1:");
            foreach (object value in values)
            {
                Console.WriteLine(value.ToString());
            }

            // Crea otra validación en la celda B1 con valores diferentes
            Validation validation2 = worksheet.Cells["B1"].GetValidation();
            validation2.Type = ValidationType.List;
            validation2.Value1 = new object[] { "Yes", "No", "Maybe" };

            // Obtén y muestra los valores de la segunda validación
            object[] values2 = validation2.Value1 as object[];
            Console.WriteLine("\nValidation values in B1:");
            foreach (object value in values2)
            {
                Console.WriteLine(value.ToString());
            }
        }
    }
}
```

### Ver también

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


