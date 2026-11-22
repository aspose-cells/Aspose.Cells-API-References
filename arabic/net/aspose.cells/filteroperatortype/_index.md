---
title: "التعداد FilterOperatorType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.FilterOperatorType. نوع عامل تصفية مخصص"
type: docs
url: /ar/net/aspose.cells/filteroperatortype/
---
## FilterOperatorType enumeration

نوع عامل الفلتر المخصص.

```csharp
public enum FilterOperatorType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| LessOrEqual | `0` | يمثل عامل LessOrEqual. |
| LessThan | `1` | يمثل عامل LessThan. |
| Equal | `2` | يمثل عامل Equal. |
| GreaterThan | `3` | يمثل عامل GreaterThan. |
| NotEqual | `4` | يمثل عامل NotEqual. |
| GreaterOrEqual | `5` | يمثل عامل GreaterOrEqual. |
| None | `6` | يمثل عدم وجود مقارنة. |
| BeginsWith | `7` | يبدأ بالنص. |
| EndsWith | `8` | ينتهي بالنص. |
| Contains | `9` | يحتوي على النص. |
| NotContains | `10` | لا يحتوي على النص. |
| NotBeginsWith | `11` | لا يبدأ بالنص. |
| NotEndsWith | `12` | لا ينتهي بالنص. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFilterOperatorTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Names");
            worksheet.Cells["A2"].PutValue("Bob");
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["A4"].PutValue("Bobby");
            worksheet.Cells["A5"].PutValue("Tom");
            
            // تعيين نطاق الفلتر التلقائي
            worksheet.AutoFilter.Range = "A1:A5";
            
            // تطبيق فلتر مخصص لإظهار الأسماء التي تبدأ بـ "Bo"
            worksheet.AutoFilter.Custom(0, FilterOperatorType.BeginsWith, "Bo");
            
            // تحديث الفلتر
            worksheet.AutoFilter.Refresh();
            
            // احفظ المصنف
            workbook.Save("FilterOperatorTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


