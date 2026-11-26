---
title: "Cell.DoubleValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Obtiene el valor double contenido en la celda"
type: docs
url: /es/net/aspose.cells/cell/doublevalue/
---
## Cell.DoubleValue property

Obtiene el valor double contenido en la celda.

```csharp
public double DoubleValue { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyDoubleValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establezca diferentes tipos de valores en las celdas
            cells["A1"].PutValue(1); // Int value
            cells["A2"].PutValue(true); // Bool value
            cells["A3"].PutValue("abc"); // String value
            cells["A4"].PutValue(false); // Bool value
            cells["A5"].PutValue(2.56); // Double value

            // Demuestre la propiedad DoubleValue
            Console.WriteLine("Double value from cell A5: " + cells["A5"].DoubleValue);
            
            // Verifique que otros tipos de valores pueden leerse como double
            Console.WriteLine("Int as double from A1: " + cells["A1"].DoubleValue);
            Console.WriteLine("Bool as double from A2: " + cells["A2"].DoubleValue);
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


