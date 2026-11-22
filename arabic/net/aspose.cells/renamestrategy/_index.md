---
title: "تعداد RenameStrategy"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.RenameStrategy. خيار الإستراتيجية لأسماء الأعمدة المكررة"
type: docs
url: /ar/net/aspose.cells/renamestrategy/
---
## RenameStrategy enumeration

خيار الاستراتيجية لأسماء الأعمدة المكررة.

```csharp
public enum RenameStrategy
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Exception | `0` | يرمي استثناءً. |
| Digit | `1` | مسمى بالرقم. ستصبح الأسماء المكررة ...1، ...2، إلخ. |
| Letter | `2` | مسمى بالحرف.. ستصبح الأسماء المكررة ...A، ...B، إلخ. |

### ملاحظات

عند معالجة البيانات مع رؤوس الأعمدة، تتطلب بعض السيناريوهات عدم تكرار الرؤوس لجميع الأعمدة. على سبيل المثال، عند تصدير البيانات إلى جدول بيانات ويتطلب أن يُؤخذ الرأس كاسم عمود جدول البيانات، تكون قيم الرؤوس المكررة غير صالحة. في مثل هذه الحالات، يمكن للمستخدم تحديد كيفية التعامل معها عن طريق تحديد هذه الإستراتيجية.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RenameStrategyDemo
    {
        public static void RenameStrategyExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات النموذجية إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("John");

            // إنشاء ExportTableOptions وتعيين RenameStrategy
            ExportTableOptions options = new ExportTableOptions
            {
                RenameStrategy = RenameStrategy.Digit // Use the Digit strategy for duplicate names
            };

            // تصدير بيانات ورقة العمل إلى DataTable
            System.Data.DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 4, 1, options);

            // عرض محتوى DataTable
            foreach (System.Data.DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item + "\t");
                }
                Console.WriteLine();
            }

            // احفظ المصنف
            workbook.Save("RenameStrategyExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


