---
title: "Cell.GetWidthOfValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Değerin genişliğini piksel biriminde alır"
type: docs
url: /tr/net/aspose.cells/cell/getwidthofvalue/
---
## Cell.GetWidthOfValue method

Değerin piksel birimindeki genişliğini alır.

```csharp
public int GetWidthOfValue()
```

### Örnekler

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

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


