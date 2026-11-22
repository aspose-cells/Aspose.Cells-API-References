---
title: "Cell.GetRichValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. تحصل على القيمة الغنية للخلية"
type: docs
url: /ar/net/aspose.cells/cell/getrichvalue/
---
## Cell.GetRichValue method

يحصل على القيمة الغنية للخلية.

```csharp
public CellRichValue GetRichValue()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetRichValueDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet ws = wb.Worksheets[0];
            
            // حدد قيمة نص غني في الخلية A1
            ws.Cells["A1"].PutValue("This is rich text");
            
            // احصل على القيمة الغنية من الخلية A1
            CellRichValue richValue = ws.Cells["A1"].GetRichValue();
            
            // اعرض قيمة النص الغني
            Console.WriteLine("Rich Text Value: " + ws.Cells["A1"].StringValue);
            
            // احفظ المصنف
            wb.Save("RichValueDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CellRichValue](../../cellrichvalue/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


