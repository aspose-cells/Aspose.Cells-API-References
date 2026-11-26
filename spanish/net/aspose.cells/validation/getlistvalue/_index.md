---
title: "Validation.GetListValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Validation. Obtener el valor de la lista de la validación para la celda especificada"
type: docs
url: /es/net/aspose.cells/validation/getlistvalue/
---
## Validation.GetListValue method

Obtenga el valor de la lista de validación para la celda especificada.

```csharp
public object GetListValue(int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | El índice de fila. |
| columna | Int32 | El índice de columna. |

### Valor de retorno

El valor para generar la lista de esta validación para la celda especificada. Si la lista hace referencia a un rango, entonces el valor devuelto será un objeto [`ReferredArea`](../../referredarea/); de lo contrario, el valor devuelto puede ser null, object[], o un objeto simple.

### Observaciones

Solo para validaciones cuyo tipo es List y que se han aplicado a la celda dada; de lo contrario se devolverá null.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodGetListValueWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la validación
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            worksheet.Cells["A4"].PutValue("Date");

            // Crear validación para la celda B1
            Validation validation = worksheet.Cells["B1"].GetValidation();
            validation.Type = ValidationType.List;
            validation.Formula1 = "A1:A4";

            // Probar GetListValue con diferentes parámetros
            Console.WriteLine("List values:");
            for (int i = 0; i < 4; i++)
            {
                object value = validation.GetListValue(i, 0);
                Console.WriteLine($"Index {i}: {value}");
            }

            // Cambiar a valores separados por comas
            validation.Formula1 = "Red,Green,Blue";
            Console.WriteLine("\nComma-separated values:");
            for (int i = 0; i < 3; i++)
            {
                object[] values = (object[])validation.GetListValue(i, 0);
                Console.WriteLine($"Index {i}: {string.Join(", ", values)}");
            }

            // Cambiar a valor único
            validation.Formula1 = "SingleValue";
            Console.WriteLine("\nSingle value:");
            object singleValue = validation.GetListValue(0, 0);
            Console.WriteLine($"Value: {singleValue}");
        }
    }
}
```

### Ver también

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


