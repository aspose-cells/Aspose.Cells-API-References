---
title: "Cells.ConvertStringToNumericValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Convierte todos los datos de tipo cadena en la hoja de cálculo a valor numérico si es posible"
type: docs
url: /es/net/aspose.cells/cells/convertstringtonumericvalue/
---
## Cells.ConvertStringToNumericValue method

Convierte todos los datos de tipo cadena en la hoja de cálculo a valor numérico si es posible.

```csharp
public void ConvertStringToNumericValue()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodConvertStringToNumericValueDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Coloque valores de cadena que pueden convertirse a valores numéricos
            cells[0, 0].PutValue("1.23");
            cells[0, 1].PutValue("1.24");
            cells[0, 2].PutValue("1.23");
            cells[0, 3].PutValue("6/20/2021");
            cells[0, 4].PutValue("def"); // This will remain as string
            cells[0, 5].PutValue("6/20/2021");

            // Convertir valores de cadena a numéricos cuando sea posible
            cells.ConvertStringToNumericValue();

            // Mostrar los valores convertidos
            Console.WriteLine("A1: " + cells[0, 0].DoubleValue);
            Console.WriteLine("B1: " + cells[0, 1].DoubleValue);
            Console.WriteLine("C1: " + cells[0, 2].DoubleValue);
            Console.WriteLine("D1: " + cells[0, 3].DoubleValue);
            Console.WriteLine("E1: " + cells[0, 4].StringValue); // Remains as string
            Console.WriteLine("F1: " + cells[0, 5].DoubleValue);
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


