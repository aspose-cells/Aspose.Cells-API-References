---
title: "CustomFilterCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CustomFilterCollection. تحصل على المرشح المخصص في الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells/customfiltercollection/item/
---
## CustomFilterCollection indexer

يحصل على الفلتر المخصص في الفهرس المحدد.

```csharp
public CustomFilter this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].Value = "Numbers";
            worksheet.Cells["A2"].Value = 10;
            worksheet.Cells["A3"].Value = 20;
            worksheet.Cells["A4"].Value = 30;
            worksheet.Cells["A5"].Value = 40;
            worksheet.Cells["A6"].Value = 50;

            try
            {
                // إنشاء CustomFilterCollection جديد
                CustomFilterCollection filters = new CustomFilterCollection();

                // الوصول إلى خاصية Item (للقراءة فقط) باستخدام الفهرس
                // نظرًا لأن المجموعة فارغة، سنقوم فقط بعرض كيفية الوصول إلى الخاصية
                // في سيناريو واقعي، ستضيف المرشحات أولاً بوسائل أخرى
                if (filters.Count > 0)
                {
                    CustomFilter firstFilter = filters[0];
                    Console.WriteLine($"First filter operator: {firstFilter.FilterOperatorType}");
                    Console.WriteLine($"First filter criteria: {firstFilter.Criteria}");
                }
                else
                {
                    Console.WriteLine("No filters in collection to demonstrate Item property");
                }

                // احفظ المصنف
                workbook.Save("CustomFilterCollectionItemDemo.xlsx");
                Console.WriteLine("CustomFilterCollection Item property demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating Item property: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [CustomFilter](../../customfilter/)
* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


