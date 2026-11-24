---
title: "Cell.GetWidthOfValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Ermittelt die Breite des Werts in Pixeln."
type: docs
url: /de/net/aspose.cells/cell/getwidthofvalue/
---
## Cell.GetWidthOfValue method

Liefert die Breite des Werts in der Einheit Pixel.

```csharp
public int GetWidthOfValue()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetWidthOfValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            cell.PutValue("CellsJava40307");
            int width = cell.GetWidthOfValue();
            
            Console.WriteLine("Width of the cell value: " + width);
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


