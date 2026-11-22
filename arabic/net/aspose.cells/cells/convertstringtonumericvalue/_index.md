---
title: "Cells.ConvertStringToNumericValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تحول جميع البيانات النصية في ورقة العمل إلى قيمة رقمية إذا أمكن"
type: docs
url: /ar/net/aspose.cells/cells/convertstringtonumericvalue/
---
## Cells.ConvertStringToNumericValue method

يحوِّل جميع بيانات السلسلة في ورقة العمل إلى قيمة رقمية إذا أمكن.

```csharp
public void ConvertStringToNumericValue()
```

### أمثلة

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
            
            // ضع القيم النصية التي يمكن تحويلها إلى قيم رقمية
            cells[0, 0].PutValue("1.23");
            cells[0, 1].PutValue("1.24");
            cells[0, 2].PutValue("1.23");
            cells[0, 3].PutValue("6/20/2021");
            cells[0, 4].PutValue("def"); // This will remain as string
            cells[0, 5].PutValue("6/20/2021");

            // حوّل القيم النصية إلى رقمية حيثما أمكن
            cells.ConvertStringToNumericValue();

            // اعرض القيم المحوّلة
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

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


