---
title: "CellsHelper.GetDateTimeFromDouble"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CellsHelper. Convierte el valor double al valor de fecha y hora"
type: docs
url: /es/net/aspose.cells/cellshelper/getdatetimefromdouble/
---
## CellsHelper.GetDateTimeFromDouble method

Convierte el valor double al valor de fecha y hora.

```csharp
public static DateTime GetDateTimeFromDouble(double doubleValue, bool date1904)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| doubleValue | Double | El valor double. |
| date1904 | Booleano | Sistema de fecha 1904. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodGetDateTimeFromDoubleWithDoubleBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepare datos para los parámetros del método (Double, Boolean)
            double doubleValue = 44197.5; // Represents 2021-01-01 12:00:00 in Excel serial date format
            bool date1904 = false; // Using 1900 date system

            try
            {
                // Llame al método GetDateTimeFromDouble con los tipos de parámetros específicos
                DateTime result = CellsHelper.GetDateTimeFromDouble(doubleValue, date1904);
                
                // Mostrar el resultado
                Console.WriteLine($"Converted DateTime: {result}");
                
                // Escriba el resultado en una celda
                worksheet.Cells["A1"].PutValue("Original Double Value:");
                worksheet.Cells["B1"].PutValue(doubleValue);
                worksheet.Cells["A2"].PutValue("Converted DateTime:");
                worksheet.Cells["B2"].PutValue(result.ToString());
                
                Console.WriteLine("Method executed successfully with parameters (Double, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetDateTimeFromDouble method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("MethodGetDateTimeFromDoubleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


