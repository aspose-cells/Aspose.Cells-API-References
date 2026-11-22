---
title: "QueryTable.PreserveFormatting"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية QueryTable. تُعيد أو تُعيّن PreserveFormatting للكائن"
type: docs
url: /ar/net/aspose.cells/querytable/preserveformatting/
---
## QueryTable.PreserveFormatting property

يعيد أو يضبط PreserveFormatting للكائن.

```csharp
public bool PreserveFormatting { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyPreserveFormattingDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة وتنسيق
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(800);

            // تطبيق التنسيق على نطاق البيانات
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;
            
            // تطبيق النمط على كل خلية في النطاق
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["B1"].SetStyle(style);

            // أنشئ جدول استعلام (محاكاة لأن الإنشاء الفعلي يتطلب مصدر بيانات خارجي)
            // في الاستخدام الفعلي، ستقوم بإنشاء هذا من اتصال خارجي
            QueryTable queryTable = worksheet.QueryTables[0];

            // عرض قيمة PreserveFormatting الحالية
            Console.WriteLine("Initial PreserveFormatting value: " + queryTable.PreserveFormatting);

            // ضبط PreserveFormatting إلى false (لن يحافظ على التنسيق الحالي أثناء التحديث)
            queryTable.PreserveFormatting = false;
            Console.WriteLine("PreserveFormatting set to: " + queryTable.PreserveFormatting);

            // محاكاة تحديث جدول الاستعلام (عادةً ما يتم مسح التنسيق عندما يكون PreserveFormatting false)
            // في سيناريو حقيقي، سيحدث هذا عندما يقوم جدول الاستعلام بتحديث بياناته
            Console.WriteLine("After refresh with PreserveFormatting=false, formatting would be lost");

            // ضبط PreserveFormatting إلى true
            queryTable.PreserveFormatting = true;
            Console.WriteLine("PreserveFormatting set to: " + queryTable.PreserveFormatting);

            // محاكاة التحديث مرة أخرى (سيحافظ الآن على التنسيق)
            Console.WriteLine("After refresh with PreserveFormatting=true, formatting is preserved");

            // احفظ المصنف
            workbook.Save("QueryTablePreserveFormattingDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


