---
title: "Cell.GetWidthOfValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. تحصل على عرض القيمة بوحدة البكسل"
type: docs
url: /ar/net/aspose.cells/cell/getwidthofvalue/
---
## Cell.GetWidthOfValue method

يحصل على عرض القيمة بوحدة البكسل.

```csharp
public int GetWidthOfValue()
```

### أمثلة

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

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


