---
title: "Cell.GetWidthOfValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Ottiene la larghezza del valore in unità di pixel"
type: docs
url: /it/net/aspose.cells/cell/getwidthofvalue/
---
## Cell.GetWidthOfValue method

Ottiene la larghezza del valore in unità di pixel.

```csharp
public int GetWidthOfValue()
```

### Esempi

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

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


