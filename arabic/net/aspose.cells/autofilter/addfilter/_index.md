---
title: "AutoFilter.AddFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AutoFilter. يضيف مرشحًا لعمود الفلتر"
type: docs
url: /ar/net/aspose.cells/autofilter/addfilter/
---
## AutoFilter.AddFilter method

يضيف مرشحًا لعمود الفلتر.

```csharp
public void AddFilter(int fieldIndex, string criteria)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | Int32 | الإزاحة الصحيحة للحقول التي تريد بناء الفلتر عليها (من اليسار في القائمة؛ الحقل الأيسر هو الحقل 0). |
| معايير | String | المعيار المحدد (سلسلة نصية؛ على سبيل المثال، "101"). يمكن أن يكون إما null أو أحد قيم الخلايا في هذا العمود فقط. |

### ملاحظات

يدعم MS Excel 2007 اختيارًا متعددًا في عمود الفلتر.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodAddFilterWithInt32StringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");
            worksheet.Cells["A5"].PutValue("Date");
            worksheet.Cells["A6"].PutValue("Elderberry");
            
            // إنشاء نطاق الفلتر التلقائي
            worksheet.AutoFilter.Range = "A1:A6";
            
            // الحصول على الفلتر التلقائي
            AutoFilter filter = worksheet.AutoFilter;
            
            // إضافة مرشحات للقيم التي تبدأ بـ 'A' و 'E'
            filter.AddFilter(0, "A*");
            filter.AddFilter(0, "E*");
            
            // تحديث الفلتر
            filter.Refresh();
            
            // احفظ المصنف
            workbook.Save("AutoFilterAddFilterDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


