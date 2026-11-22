---
title: "ListObject.HasAutoFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListObject. تشير إلى ما إذا كان تم تطبيق الفلتر التلقائي على هذا الجدول"
type: docs
url: /ar/net/aspose.cells.tables/listobject/hasautofilter/
---
## ListObject.HasAutoFilter property

يشير إلى ما إذا كان الفلتر التلقائي مطبقًا على هذا الجدول.

```csharp
public bool HasAutoFilter { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Tables;

    public class ListObjectPropertyHasAutoFilterDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء بيانات عينة للجدول
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("Alice");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Bob");
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["A4"].PutValue("Charlie");
            worksheet.Cells["B4"].PutValue(78);

            try
            {
                // إضافة ListObject (جدول) يغطي نطاق البيانات
                int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
                ListObject listObject = worksheet.ListObjects[tableIndex];

                // التأكد من أن الجدول تم تغيير حجمه لتضمين جميع الصفوف
                listObject.Resize(0, 0, 4, 2, true);

                // قراءة وعرض قيمة خاصية HasAutoFilter
                bool hasFilter = listObject.HasAutoFilter;
                Console.WriteLine("HasAutoFilter: " + hasFilter);

                // يمكن الوصول إلى كائن AutoFilter عبر خاصية AutoFilter
                // إظهار أنه ليس فارغًا عندما تكون HasAutoFilter صحيحة
                if (hasFilter && listObject.AutoFilter != null)
                {
                    // تطبيق فلتر بسيط على العمود \"Score\" (الفهرس 1) لإظهار الصفوف التي يكون فيها Score >= 80
                    listObject.AutoFilter.Filter(1, ">=80");

                    Console.WriteLine("Filtered rows (Score >= 80):");
                    for (int row = 1; row <= 4; row++)
                    {
                        // استخدام Cells.Rows للتحقق مما إذا كان الصف مخفيًا
                        if (!worksheet.Cells.Rows[row].IsHidden)
                        {
                            Console.WriteLine($"{worksheet.Cells[row, 0].StringValue} - {worksheet.Cells[row, 1].IntValue}");
                        }
                    }

                    // مسح الفلتر
                    listObject.AutoFilter.RemoveFilter(1);
                }

                // احفظ دفتر العمل (اختياري)
                workbook.Save("HasAutoFilterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### انظر أيضًا

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


