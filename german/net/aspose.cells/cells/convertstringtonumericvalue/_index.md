---
title: "Cells.ConvertStringToNumericValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Konvertiert alle Zeichenkettendaten im Arbeitsblatt nach Möglichkeit in numerische Werte"
type: docs
url: /de/net/aspose.cells/cells/convertstringtonumericvalue/
---
## Cells.ConvertStringToNumericValue method

Konvertiert alle Zeichenkettendaten im Arbeitsblatt, wenn möglich, in numerische Werte.

```csharp
public void ConvertStringToNumericValue()
```

### Beispiele

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
            
            // Füge Zeichenkettenwerte ein, die in numerische Werte konvertiert werden können
            cells[0, 0].PutValue("1.23");
            cells[0, 1].PutValue("1.24");
            cells[0, 2].PutValue("1.23");
            cells[0, 3].PutValue("6/20/2021");
            cells[0, 4].PutValue("def"); // This will remain as string
            cells[0, 5].PutValue("6/20/2021");

            // Konvertiere Zeichenkettenwerte nach Möglichkeit in numerische Werte
            cells.ConvertStringToNumericValue();

            // Zeige die konvertierten Werte an
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

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


