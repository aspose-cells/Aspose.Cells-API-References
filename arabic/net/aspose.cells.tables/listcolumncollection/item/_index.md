---
title: "ListColumnCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListColumnCollection. تحصل على ListColumn حسب الفهرس"
type: docs
url: /ar/net/aspose.cells.tables/listcolumncollection/item/
---
## ListColumnCollection indexer (1 of 2)

يحصل على ListColumn حسب الفهرس.

```csharp
public ListColumn this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس. |

### قيمة الإرجاع

كائن ListColumn.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("T1");
            worksheet.Cells["B1"].PutValue("T2");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(2);

            // إنشاء كائن قائمة
            int index = worksheet.ListObjects.Add(0, 0, 1, 1, true);
            ListObject listObj = worksheet.ListObjects[index];
            
            // الوصول إلى أعمدة القائمة باستخدام خاصية Item
            ListColumn firstColumn = listObj.ListColumns[0];
            Console.WriteLine("First column name: " + firstColumn.Name);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ListColumn](../../listcolumn/)
* class [ListColumnCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## ListColumnCollection indexer (2 of 2)

يحصل على ListColumn حسب الاسم.

```csharp
public ListColumn this[string name] { get; }
```

| معامل | الوصف |
| --- | --- |
| name | اسم ListColumn |

### قيمة الإرجاع

كائن ListColumn.

### انظر أيضًا

* class [ListColumn](../../listcolumn/)
* class [ListColumnCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


