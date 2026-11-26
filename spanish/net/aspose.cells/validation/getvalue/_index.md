---
title: "Validation.GetValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Validation. Obtenga el valor de la validación en la celda específica"
type: docs
url: /es/net/aspose.cells/validation/getvalue/
---
## Validation.GetValue method

Obtenga el valor de la validación en la celda específica.

```csharp
public object GetValue(int row, int column, bool isValue1)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | El índice de fila. |
| columna | Int32 | El índice de columna. |
| isValue1 | Booleano | Indica si se está obteniendo el primer valor. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodGetValueWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra y validación
            worksheet.Cells["A1"].PutValue("Select Item:");
            worksheet.Cells["B1"].PutValue("Item 1");
            worksheet.Cells["B2"].PutValue("Item 2");
            
            // Crear validación para la celda B1
            Validation validation = worksheet.Cells["B1"].GetValidation();
            validation.Type = ValidationType.List;
            validation.Formula1 = "A1:B2";
            
            // Obtener valor usando el método GetValue con los parámetros fila, columna y convertir numérico a fecha
            object value = validation.GetValue(0, 1, false);
            
            // Mostrar el resultado
            Console.WriteLine("Validation value: " + value.ToString());
        }
    }
}
```

### Ver también

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


