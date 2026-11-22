---
title: "ListObject.AutoFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListObject. تحصل على الفلتر التلقائي لهذا الجدول"
type: docs
url: /ar/net/aspose.cells.tables/listobject/autofilter/
---
## ListObject.AutoFilter property

يحصل على الفلتر التلقائي لهذا الجدول.

```csharp
public AutoFilter AutoFilter { get; }
```

### ملاحظات

يعمل فقط عندما [`HasAutoFilter`](../hasautofilter/) يكون false.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyAutoFilterDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Mary");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Peter");
            worksheet.Cells["B4"].PutValue(35);

            // إنشاء ListObject
            int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject listObject = worksheet.ListObjects[index];

            // تغيير حجم كائن القائمة لتضمين جميع البيانات
            listObject.Resize(0, 0, 4, 2, true);

            // الوصول إلى وإظهار وظيفة AutoFilter
            if (listObject.AutoFilter != null)
            {
                // تطبيق الفلتر على عمود العمر (العمود 2)
                listObject.AutoFilter.Filter(1, "25");
                
                // عرض البيانات المفلترة
                Console.WriteLine("Filtered Data:");
                for (int row = 1; row <= 4; row++)
                {
                    if (!worksheet.Cells.Rows[row].IsHidden)
                    {
                        Console.WriteLine($"{worksheet.Cells[row, 0].StringValue} - {worksheet.Cells[row, 1].IntValue}");
                    }
                }

                // مسح الفلتر
                listObject.AutoFilter.RemoveFilter(1);
            }

            // احفظ المصنف
            workbook.Save("ListObjectAutoFilterDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [AutoFilter](../../../aspose.cells/autofilter/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


