---
title: "AutoFilter.Refresh"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AutoFilter. تحديث مرشحات AutoFilter لإخفاء أو إظهار الصفوف"
type: docs
url: /ar/net/aspose.cells/autofilter/refresh/
---
## Refresh() {#refresh}

تحديث الفلاتر التلقائية لإخفاء أو إظهار الصفوف.

```csharp
public int[] Refresh()
```

### قيمة الإرجاع

يعيد جميع فهارس الصفوف المخفية.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodRefreshDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["B6"].PutValue("Header1");
            worksheet.Cells["C6"].PutValue("Header2");
            worksheet.Cells["D6"].PutValue("Header3");
            worksheet.Cells["E6"].PutValue("Values");
            
            for (int i = 7; i <= 15; i++)
            {
                worksheet.Cells["B" + i].PutValue("Item " + (i-6));
                worksheet.Cells["E" + i].PutValue((i-6) * 100);
            }

            // تطبيق الفلتر التلقائي
            worksheet.AutoFilter.Range = "B6:E6";
            
            // تصفية القيم الأكبر من 500
            worksheet.AutoFilter.Custom(3, FilterOperatorType.GreaterThan, 500);
            worksheet.AutoFilter.Refresh();
            
            Console.WriteLine("Row 7 hidden: " + worksheet.Cells.IsRowHidden(7));
            Console.WriteLine("Row 13 hidden: " + worksheet.Cells.IsRowHidden(13));
            
            // تغيير الفلتر لإظهار القيم التي تساوي 500 أو أكبر من 700
            worksheet.AutoFilter.Custom(3, FilterOperatorType.Equal, 500, false, FilterOperatorType.GreaterThan, 700);
            worksheet.AutoFilter.Refresh();
            
            Console.WriteLine("After refresh - Row 7 hidden: " + worksheet.Cells.IsRowHidden(7));
            Console.WriteLine("After refresh - Row 13 hidden: " + worksheet.Cells.IsRowHidden(13));
        }
    }
}
```

### انظر أيضًا

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Refresh(bool) {#refresh_1}

يحصل على مؤشرات جميع الصفوف المخفية.

```csharp
public int[] Refresh(bool hideRows)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| hideRows | منطقي | إذا كان صحيحًا، إخفاء الصفوف المصفاة. |

### قيمة الإرجاع

يعيد جميع فهارس الصفوف المخفية.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodRefreshWithBooleanDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(1);
            worksheet.Cells["A5"].PutValue(3);
            
            // تطبيق الفلتر التلقائي
            worksheet.AutoFilter.Range = "A1:A5";
            worksheet.AutoFilter.AddFilter(0, "1"); // Filter to show only rows with value 1
            
            // تحديث الفلتر والحصول على الصفوف المخفية
            int[] hiddenRows = worksheet.AutoFilter.Refresh(false);
            
            Console.WriteLine("Hidden rows after filter:");
            if (hiddenRows != null)
            {
                foreach (int row in hiddenRows)
                {
                    Console.WriteLine(row);
                }
            }
            
            // إظهار جميع البيانات وتحديث مرة أخرى
            worksheet.AutoFilter.ShowAll();
            hiddenRows = worksheet.AutoFilter.Refresh(false);
            
            Console.WriteLine("\nHidden rows after showing all:");
            if (hiddenRows == null)
            {
                Console.WriteLine("No hidden rows");
            }
        }
    }
}
```

### انظر أيضًا

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


