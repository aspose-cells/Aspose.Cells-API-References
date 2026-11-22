---
title: "QueryTableCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية QueryTableCollection. الحصول على جدول الاستعلام بواسطة الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells/querytablecollection/item/
---
## QueryTableCollection indexer

يحصل على الـ querytable بالفهرس المحدد.

```csharp
public QueryTable this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس. |

### قيمة الإرجاع

جدول الاستعلام

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTableCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى QueryTableCollection
            QueryTableCollection queryTables = worksheet.QueryTables;

            try
            {
                // التحقق مما إذا كان هناك أي QueryTables
                if (queryTables.Count > 0)
                {
                    // الوصول إلى أول QueryTable باستخدام خاصية Item
                    QueryTable firstQueryTable = queryTables[0];
                    Console.WriteLine("First QueryTable accessed successfully.");

                    // عرض بعض خصائص QueryTable
                    Console.WriteLine("QueryTable Name: " + firstQueryTable.Name);
                }
                else
                {
                    Console.WriteLine("No QueryTables found in the worksheet.");
                }

                // احفظ المصنف
                workbook.Save("QueryTableItemDemo.xlsx");
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

* class [QueryTable](../../querytable/)
* class [QueryTableCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


