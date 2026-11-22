---
title: "Cell.R1C1Formula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. تحصل أو تعين صيغة R1C1 للخلية"
type: docs
url: /ar/net/aspose.cells/cell/r1c1formula/
---
## Cell.R1C1Formula property

تحصل أو تعين صيغة R1C1 للـ [`Cell`](../).

```csharp
public string R1C1Formula { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyR1C1FormulaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين قيمة A1
            worksheet.Cells["A1"].PutValue(10);
            
            // تعيين قيمة B1
            worksheet.Cells["B1"].PutValue(20);
            
            // تعيين صيغة C1 بصيغة A1
            worksheet.Cells["C1"].Formula = "=A1+B1";
            
            // احصل على صيغة R1C1 وعرضها
            string r1c1Formula = worksheet.Cells["C1"].R1C1Formula;
            Console.WriteLine("R1C1 Formula: " + r1c1Formula);
            
            // تعيين صيغة D1 بصيغة R1C1
            worksheet.Cells["D1"].R1C1Formula = "=RC[-3]+RC[-2]";
            
            // احصل على صيغة A1 وعرضها
            string a1Formula = worksheet.Cells["D1"].Formula;
            Console.WriteLine("A1 Formula: " + a1Formula);
            
            // احفظ المصنف
            workbook.Save("R1C1FormulaDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


