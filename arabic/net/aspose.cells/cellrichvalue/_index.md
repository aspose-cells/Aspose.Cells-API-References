---
title: "الفئة CellRichValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.CellRichValue. تمثّل القيمة الغنية للخلية"
type: docs
url: /ar/net/aspose.cells/cellrichvalue/
---
## CellRichValue class

يمثل القيمة الغنية للخلية.

```csharp
public abstract class CellRichValue
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| virtual [AltText](../../aspose.cells/cellrichvalue/alttext/) { get; set; } | يحصل على النص البديل المرتبط بالصورة. |
| virtual [ErrorValue](../../aspose.cells/cellrichvalue/errorvalue/) { get; } | يحصل على نوع قيمة الخطأ للخلية. |
| virtual [Image](../../aspose.cells/cellrichvalue/image/) { get; } | يحصل على بيانات الصورة للخلية. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassCellRichValueDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // عيّن قيمة غنية في الخلية A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Rich Value");
            
            // احصل على القيمة الغنية من الخلية A1
            CellRichValue richValue = cell.GetRichValue();
            
            // اعرض خصائص القيمة الغنية
            Console.WriteLine("Rich Value: " + richValue.ToString());
            
            // احفظ المصنف
            workbook.Save("RichValueDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


