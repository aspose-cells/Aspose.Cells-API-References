---
title: "QueryTable.AdjustColumnWidth"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية QueryTable. تُعيد أو تُعيّن AdjustColumnWidth للكائن"
type: docs
url: /ar/net/aspose.cells/querytable/adjustcolumnwidth/
---
## QueryTable.AdjustColumnWidth property

يعيد أو يضبط AdjustColumnWidth للكائن.

```csharp
public bool AdjustColumnWidth { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyAdjustColumnWidthDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة بأعمدة ذات عرض متغيّر
            worksheet.Cells["A1"].PutValue("Narrow Column");
            worksheet.Cells["B1"].PutValue("Wide Column Data");
            worksheet.Cells["A2"].PutValue("Short");
            worksheet.Cells["B2"].PutValue("This is some very long text that should demonstrate column width adjustment");

            // عيّن عرض الأعمدة يدويًا
            worksheet.Cells.SetColumnWidth(0, 10); // Narrow column
            worksheet.Cells.SetColumnWidth(1, 10); // Initially narrow for wide data

            // أنشئ جدول استعلام (محاكاة لأن الإنشاء الفعلي يتطلب مصدر بيانات خارجي)
            QueryTable queryTable = worksheet.QueryTables[0];

            // اعرض قيمة AdjustColumnWidth الحالية
            Console.WriteLine("Initial AdjustColumnWidth value: " + queryTable.AdjustColumnWidth);

            // عيّن AdjustColumnWidth إلى true وأظهر التأثير
            queryTable.AdjustColumnWidth = true;
            Console.WriteLine("AdjustColumnWidth set to: " + queryTable.AdjustColumnWidth);
            Console.WriteLine("After setting to true, columns would auto-adjust to fit content during refresh");

            // حاكي تحديث جدول الاستعلام (عادةً ما يضبط عرض الأعمدة)
            // في سيناريو حقيقي، سيحدث هذا عندما يقوم جدول الاستعلام بتحديث بياناته
            Console.WriteLine("Column widths after refresh with AdjustColumnWidth=true:");
            Console.WriteLine("Column A width: " + worksheet.Cells.GetColumnWidth(0));
            Console.WriteLine("Column B width: " + worksheet.Cells.GetColumnWidth(1));

            // عيّن AdjustColumnWidth إلى false وأظهر التأثير
            queryTable.AdjustColumnWidth = false;
            Console.WriteLine("AdjustColumnWidth set to: " + queryTable.AdjustColumnWidth);

            // حاكي التحديث مرة أخرى (سيحافظ الآن على عرض الأعمدة الأصلي)
            Console.WriteLine("Column widths after refresh with AdjustColumnWidth=false:");
            Console.WriteLine("Column A width remains: " + worksheet.Cells.GetColumnWidth(0));
            Console.WriteLine("Column B width remains: " + worksheet.Cells.GetColumnWidth(1));

            // احفظ المصنف
            workbook.Save("QueryTableAdjustColumnWidthDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


