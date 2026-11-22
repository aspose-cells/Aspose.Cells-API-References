---
title: "AutoFilter.RemoveFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AutoFilter. تزيل مرشحًا لعمود مرشح"
type: docs
url: /ar/net/aspose.cells/autofilter/removefilter/
---
## RemoveFilter(int, string) {#removefilter_1}

يزيل مرشحًا لعمود الفلتر.

```csharp
public void RemoveFilter(int fieldIndex, string criteria)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | Int32 | الإزاحة الصحيحة للحقول التي تريد بناء الفلتر عليها (من اليسار في القائمة؛ الحقل الأيسر هو الحقل 0). |
| معايير | String | المعيار المحدد (سلسلة نصية؛ على سبيل المثال، "101"). يمكن أن يكون إما null أو أحد قيم الخلايا في هذا العمود فقط. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodRemoveFilterWithInt32StringDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد والوصول إلى ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء بيانات عينة للتوضيح
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["C1"].PutValue("Price");
            
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue("Electronics");
            worksheet.Cells["C2"].PutValue(999.99);
            
            worksheet.Cells["A3"].PutValue("Novel");
            worksheet.Cells["B3"].PutValue("Books");
            worksheet.Cells["C3"].PutValue(19.99);
            
            worksheet.Cells["A4"].PutValue("Smartphone");
            worksheet.Cells["B4"].PutValue("Electronics");
            worksheet.Cells["C4"].PutValue(599.99);

            // تعيين نطاق الفلتر التلقائي (العناوين + 3 صفوف بيانات)
            worksheet.AutoFilter.SetRange(0, 0, 2);

            try
            {
                AutoFilter autoFilter = worksheet.AutoFilter;
                
                // تطبيق مرشح على عمود الفئة (fieldIndex 1) لـ "Electronics"
                autoFilter.AddFilter(1, "Electronics");
                autoFilter.Refresh(); // Apply filter to hide non-matching rows
                
                // إزالة المرشح المحدد من عمود الفئة
                autoFilter.RemoveFilter(1, "Electronics");
                autoFilter.Refresh(); // Re-apply filter (now shows all rows)

                Console.WriteLine("RemoveFilter executed: Electronics filter removed from Category column.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // احفظ المصنف المعدل
            workbook.Save("AutoFilterMethodRemoveFilterWithInt32StringDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveFilter(int) {#removefilter}

يزيل الفلتر المحدد.

```csharp
public void RemoveFilter(int fieldIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | Int32 | مؤشر المرشح المحدد |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodRemoveFilterWithInt32Demo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("Grape");
            
            // تطبيق الفلتر التلقائي
            worksheet.AutoFilter.Range = "A1:A5";
            AutoFilter filter = worksheet.AutoFilter;
            
            // إضافة مرشح
            filter.AddFilter(0, "Apple");
            filter.Refresh();
            
            Console.WriteLine("After adding filter - Visible rows:");
            PrintVisibleRows(worksheet);
            
            // إزالة الفلتر
            filter.RemoveFilter(0);
            filter.Refresh();
            
            Console.WriteLine("\nAfter removing filter - Visible rows:");
            PrintVisibleRows(worksheet);
        }
        
        private static void PrintVisibleRows(Worksheet worksheet)
        {
            for (int i = 0; i < worksheet.Cells.MaxDataRow + 1; i++)
            {
                if (!worksheet.Cells.Rows[i].IsHidden)
                {
                    Console.WriteLine($"Row {i + 1}: {worksheet.Cells[i, 0].StringValue}");
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


