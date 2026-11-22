---
title: "Font.IsBold"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية الخط. تحصل أو تعين قيمة تشير إلى ما إذا كان الخط عريض"
type: docs
url: /ar/net/aspose.cells/font/isbold/
---
## Font.IsBold property

يحصل على أو يضبط قيمة تشير إلى ما إذا كان الخط عريضًا.

```csharp
public bool IsBold { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsBoldDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى الخلية A1 وتعيين قيمتها
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Bold Text Demo");
            
            // احصل على نمط الخلية وتعيين الخط إلى عريض
            Style style = cell.GetStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);
            
            // احفظ المصنف
            workbook.Save("FontIsBoldDemo.xlsx");
            
            // تحقق من خاصية العريض
            Workbook loadedWorkbook = new Workbook("FontIsBoldDemo.xlsx");
            Style loadedStyle = loadedWorkbook.Worksheets[0].Cells["A1"].GetStyle();
            Console.WriteLine("IsBold property: " + loadedStyle.Font.IsBold);
        }
    }
}
```

### انظر أيضًا

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


