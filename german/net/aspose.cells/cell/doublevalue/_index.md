---
title: "Cell.DoubleValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Eigenschaft. Gibt den in der Zelle enthaltenen Double-Wert zurück"
type: docs
url: /de/net/aspose.cells/cell/doublevalue/
---
## Cell.DoubleValue property

Liefert den double-Wert, der in der Zelle enthalten ist.

```csharp
public double DoubleValue { get; }
```

### Beispiele

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

            // Verschiedene Werttypen in Zellen festlegen
            cells["A1"].PutValue(1); // Int value
            cells["A2"].PutValue(true); // Bool value
            cells["A3"].PutValue("abc"); // String value
            cells["A4"].PutValue(false); // Bool value
            cells["A5"].PutValue(2.56); // Double value

            // Demonstration der DoubleValue-Eigenschaft
            Console.WriteLine("Double value from cell A5: " + cells["A5"].DoubleValue);
            
            // Überprüfen, ob andere Werttypen als Double gelesen werden können
            Console.WriteLine("Int as double from A1: " + cells["A1"].DoubleValue);
            Console.WriteLine("Bool as double from A2: " + cells["A2"].DoubleValue);
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


