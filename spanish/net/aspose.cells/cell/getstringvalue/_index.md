---
title: "Cell.GetStringValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Obtiene el valor de cadena mediante una estrategia de formato específica"
type: docs
url: /es/net/aspose.cells/cell/getstringvalue/
---
## Cell.GetStringValue method

Obtiene el valor de cadena mediante una estrategia de formato específica.

```csharp
public string GetStringValue(CellValueFormatStrategy formatStrategy)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formatStrategy | CellValueFormatStrategy | La estrategia formateada. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetStringValueWithCellValueFormatStrategyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer diferentes tipos de datos en celdas
            cells["A1"].PutValue(123.45); // Numeric value
            cells["A2"].PutValue(DateTime.Now); // DateTime value
            cells["A3"].PutValue(true); // Boolean value
            cells["A4"].PutValue("Sample Text"); // String value

            // Demostrar GetStringValue con diferentes estrategias de formato
            Console.WriteLine("None: " + cells["A1"].GetStringValue(CellValueFormatStrategy.None));
            Console.WriteLine("CellStyle: " + cells["A1"].GetStringValue(CellValueFormatStrategy.CellStyle));
            Console.WriteLine("DisplayString: " + cells["A1"].GetStringValue(CellValueFormatStrategy.DisplayString));

            Console.WriteLine("DateTime None: " + cells["A2"].GetStringValue(CellValueFormatStrategy.None));
            Console.WriteLine("DateTime CellStyle: " + cells["A2"].GetStringValue(CellValueFormatStrategy.CellStyle));
        }
    }
}
```

### Ver también

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


