---
title: "تعداد GridlineType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.GridlineType. يعدد أنواع خطوط الشبكة"
type: docs
url: /ar/net/aspose.cells/gridlinetype/
---
## GridlineType enumeration

يسرد نوع خطوط الشبكة.

```csharp
public enum GridlineType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Dotted | `0` | يمثل خطًا منقطًا. |
| Hair | `1` | يمثل خطًا رفيعًا. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassGridlineTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء خيارات الحفظ وتعيين نوع خط الشبكة
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.GridlineType = GridlineType.Dotted;
            
            // إضافة بعض البيانات التجريبية لرؤية خطوط الشبكة
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B2"].PutValue(123);
            worksheet.Cells["C3"].PutValue(DateTime.Now);
            
            // حفظ المصنف باستخدام خيارات الحفظ
            workbook.Save("GridlineTypeDemo.docx", saveOptions);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


