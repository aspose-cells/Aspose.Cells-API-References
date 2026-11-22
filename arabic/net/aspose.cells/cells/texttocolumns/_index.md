---
title: "Cells.TextToColumns"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تقسم المحتوى في العمود المحدد إلى أعمدة متعددة"
type: docs
url: /ar/net/aspose.cells/cells/texttocolumns/
---
## Cells.TextToColumns method

يقسم المحتوى في العمود المحدد إلى عدة أعمدة..

```csharp
public int TextToColumns(int row, int column, int totalRows, TxtLoadOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف. |
| عمود | Int32 | فهرس العمود. |
| totalRows | Int32 | عدد الصفوف. |
| خيارات | TxtLoadOptions | خيارات التقسيم. |

### قيمة الإرجاع

إجمالي عدد الأعمدة للقيم المقسمة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodTextToColumnsWithInt32Int32Int32TxtLoadOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // تعيين بيانات تجريبية بقيم مفصولة بفواصل
            sheet.Cells["A1"].PutValue("John,Doe,30");
            sheet.Cells["A2"].PutValue("Jane,Smith,28");

            // إنشاء خيارات تحميل النص باستخدام الفاصلة كفاصل
            TxtLoadOptions options = new TxtLoadOptions();
            options.Separator = ',';

            // تقسيم النص إلى أعمدة بدءًا من الخلية A1، بعرض 3 أعمدة
            sheet.Cells.TextToColumns(0, 0, 3, options);

            // تحقق من النتائج
            Console.WriteLine("B1: " + sheet.Cells["B1"].StringValue); // Should output "Doe"
            Console.WriteLine("C2: " + sheet.Cells["C2"].StringValue); // Should output "28"

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


