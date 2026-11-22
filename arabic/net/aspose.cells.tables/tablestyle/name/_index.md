---
title: "TableStyle.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TableStyle. تحصل على اسم نمط الجدول"
type: docs
url: /ar/net/aspose.cells.tables/tablestyle/name/
---
## TableStyle.Name property

يحصل على اسم نمط الجدول.

```csharp
public string Name { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStylePropertyNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى مجموعة أنماط الجدول
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

            try
            {
                // احصل على أول نمط جدول من المجموعة
                TableStyle tableStyle = tableStyles[0];

                // اعرض قيمة خاصية Name
                Console.WriteLine("Table Style Name: " + tableStyle.Name);

                // وضح الوصول إلى الخاصية للقراءة فقط
                string styleName = tableStyle.Name;
                Console.WriteLine("Retrieved style name: " + styleName);

                // أظهر أننا يمكننا استخدام الاسم للإشارة إلى النمط
                Console.WriteLine("This table style can be referenced by name: " + tableStyle.Name);

                // احفظ المصنف
                workbook.Save("TableStyleNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [TableStyle](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


