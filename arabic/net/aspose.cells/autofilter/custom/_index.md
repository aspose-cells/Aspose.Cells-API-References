---
title: "AutoFilter.Custom"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AutoFilter. تصفي قائمة بمعيار مخصص"
type: docs
url: /ar/net/aspose.cells/autofilter/custom/
---
## Custom(int, FilterOperatorType, object) {#custom}

يفلتر قائمة بمعيار مخصص.

```csharp
public void Custom(int fieldIndex, FilterOperatorType operatorType1, object criteria1)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | Int32 | الإزاحة الصحيحة للحقول التي تريد بناء الفلتر عليها (من اليسار في القائمة؛ الحقل الأيسر هو الحقل 0). |
| operatorType1 | FilterOperatorType | نوع عامل الفلتر |
| criteria1 | Object | المعيار المخصص |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodCustomWithInt32FilterOperatorTypeObjectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات تجريبية إلى العمود A (10 صفوف + رأس)
            worksheet.Cells["A1"].PutValue("Numbers");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i); // A2-A11: 1-10
            }

            // تعيين نطاق الفلتر التلقائي (A1:A11)
            worksheet.AutoFilter.SetRange(0, 0, 0);

            try
            {
                // تطبيق فلتر مخصص: الأرقام > 5
                worksheet.AutoFilter.Custom(0, FilterOperatorType.GreaterThan, 5);
                
                // تحديث الفلتر لتطبيق التغييرات
                worksheet.AutoFilter.Refresh();
                
                Console.WriteLine("Custom filter applied: Column 0 values > 5");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Custom method: {ex.Message}");
            }
            
            // حفظ المصنف المفلتر
            workbook.Save("AutoFilterMethodCustomWithInt32FilterOperatorTypeObjectDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [FilterOperatorType](../../filteroperatortype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Custom(int, FilterOperatorType, object, bool, FilterOperatorType, object) {#custom_1}

يفلتر قائمة بمعايير مخصصة.

```csharp
public void Custom(int fieldIndex, FilterOperatorType operatorType1, object criteria1, bool isAnd, 
    FilterOperatorType operatorType2, object criteria2)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | Int32 | الإزاحة الصحيحة للحقول التي تريد بناء الفلتر عليها (من اليسار في القائمة؛ الحقل الأيسر هو الحقل 0). |
| operatorType1 | FilterOperatorType | نوع عامل الفلتر |
| criteria1 | Object | المعيار المخصص |
| isAnd | منطقي |  |
| operatorType2 | FilterOperatorType | نوع عامل الفلتر |
| criteria2 | Object | المعيار المخصص |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodCustomWithInt32FilterOperatorTypeObjectBDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء بيانات عينة
            worksheet.Cells["A1"].PutValue("Product ID");
            worksheet.Cells["A2"].PutValue(85);
            worksheet.Cells["A3"].PutValue(42);
            worksheet.Cells["A4"].PutValue(65);
            worksheet.Cells["A5"].PutValue(95);
            worksheet.Cells["A6"].PutValue(30);
            worksheet.Cells["A7"].PutValue(75);

            // تعيين نطاق الفلتر التلقائي (A1:A7)
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.SetRange(0, 0, 0); // Start row: 0 (A1), strartt column: 0 (A), end Column: 0 (A)

            try
            {
                // تطبيق فلتر مخصص: أكبر من أو يساوي 50 و أصغر من أو يساوي 100
                autoFilter.Custom(
                    0, // Field index (column A)
                    FilterOperatorType.GreaterOrEqual,
                    50, // First criteria
                    true, // AND combination
                    FilterOperatorType.LessOrEqual,
                    100 // Second criteria
                );

                Console.WriteLine("Custom filter applied successfully with parameters: " +
                    "(Int32, FilterOperatorType, Object, Boolean, FilterOperatorType, Object)");

                // تحديث الفلاتر وحفظ النتائج
                autoFilter.Refresh();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Custom method: {ex.Message}");
            }

            // حفظ المصنف المفلتر
            workbook.Save("AutoFilterMethodCustomWithInt32FilterOperatorTypeObjectBDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [FilterOperatorType](../../filteroperatortype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


