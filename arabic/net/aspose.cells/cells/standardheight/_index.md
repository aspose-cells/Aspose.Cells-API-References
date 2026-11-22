---
title: "Cells.StandardHeight"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cells. تحصل أو تعين ارتفاع الصف الافتراضي في هذه ورقة العمل بوحدة النقاط"
type: docs
url: /ar/net/aspose.cells/cells/standardheight/
---
## Cells.StandardHeight property

يحصل أو يعيّن ارتفاع الصف الافتراضي في ورقة العمل هذه، بوحدة النقاط.

```csharp
public double StandardHeight { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardHeightDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // احصل على الارتفاع القياسي واعرضه
            double standardHeight = worksheet.Cells.StandardHeight;
            Console.WriteLine("Standard Height: " + standardHeight);
            
            // عيّن ارتفاعًا قياسيًا جديدًا
            worksheet.Cells.StandardHeight = 20;
            Console.WriteLine("New Standard Height: " + worksheet.Cells.StandardHeight);
            
            // احفظ المصنف
            workbook.Save("StandardHeightDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


