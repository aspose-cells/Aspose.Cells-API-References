---
title: "CellsHelper.GetDateTimeFromDouble"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CellsHelper. تحويل القيمة المزدوجة إلى قيمة التاريخ والوقت"
type: docs
url: /ar/net/aspose.cells/cellshelper/getdatetimefromdouble/
---
## CellsHelper.GetDateTimeFromDouble method

حوّل القيمة المزدوجة إلى قيمة تاريخ ووقت.

```csharp
public static DateTime GetDateTimeFromDouble(double doubleValue, bool date1904)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| doubleValue | Double | القيمة المزدوجة. |
| date1904 | منطقي | نظام تاريخ 1904. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodGetDateTimeFromDoubleWithDoubleBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تحضير البيانات لمعلمات الطريقة (Double, Boolean)
            double doubleValue = 44197.5; // Represents 2021-01-01 12:00:00 in Excel serial date format
            bool date1904 = false; // Using 1900 date system

            try
            {
                // استدعاء طريقة GetDateTimeFromDouble مع أنواع المعلمات المحددة
                DateTime result = CellsHelper.GetDateTimeFromDouble(doubleValue, date1904);
                
                // اعرض النتيجة
                Console.WriteLine($"Converted DateTime: {result}");
                
                // اكتب النتيجة في خلية
                worksheet.Cells["A1"].PutValue("Original Double Value:");
                worksheet.Cells["B1"].PutValue(doubleValue);
                worksheet.Cells["A2"].PutValue("Converted DateTime:");
                worksheet.Cells["B2"].PutValue(result.ToString());
                
                Console.WriteLine("Method executed successfully with parameters (Double, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetDateTimeFromDouble method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("MethodGetDateTimeFromDoubleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


