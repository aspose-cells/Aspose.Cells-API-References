---
title: "Cell.IsNumericValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Eigenschaft. Gibt an, ob der Wert dieser Zelle numerisch, int, double und datetime ist"
type: docs
url: /de/net/aspose.cells/cell/isnumericvalue/
---
## Cell.IsNumericValue property

Gibt an, ob der Wert dieser Zelle numerisch (int, double und datetime) ist

```csharp
public bool IsNumericValue { get; }
```

### Hinweise

Gilt auch für Formelfelder, um das berechnete Ergebnis zu prüfen

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsNumericValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie verschiedenen Datentypen zu Zellen hinzu
            Cell cell1 = worksheet.Cells["A1"];
            cell1.PutValue(123.45); // Numeric value

            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Hello World"); // String value

            // Überprüfen Sie, ob Zellen numerische Werte enthalten
            Console.WriteLine("Cell A1 IsNumericValue: " + cell1.IsNumericValue);
            Console.WriteLine("Cell A2 IsNumericValue: " + cell2.IsNumericValue);

            // Demonstrieren Sie die Verwendung mit bedingter Logik
            if (cell1.IsNumericValue)
            {
                Console.WriteLine("Cell A1 contains a numeric value: " + cell1.DoubleValue);
            }

            if (!cell2.IsNumericValue)
            {
                Console.WriteLine("Cell A2 does not contain a numeric value");
            }
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


