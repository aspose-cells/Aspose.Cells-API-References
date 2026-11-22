---
title: "Range.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Range. يحصل على كائن Cell في هذا النطاق"
type: docs
url: /ar/net/aspose.cells/range/item/
---
## Range indexer

يحصل على كائن [`Cell`](../../cell/) في هذا النطاق.

```csharp
public Cell this[int rowOffset, int columnOffset] { get; }
```

| معامل | الوصف |
| --- | --- |
| rowOffset | إزاحة الصف في هذا النطاق، بدءًا من الصفر. |
| columnOffset | إزاحة العمود في هذا النطاق، بدءًا من الصفر. |

### قيمة الإرجاع

[`Cell`](../../cell/) object.

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RangePropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء بيانات نموذجية
            DataTable dt = new DataTable();
            dt.Columns.Add("Id", typeof(int));
            dt.Columns.Add("Name", typeof(string));
            dt.Rows.Add(1001, "Item 1");
            dt.Rows.Add(1002, "Item 2");

            // إنشاء نطاق وعرض خاصية Item
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B3");
            
            // تعيين رؤوس باستخدام خاصية Item
            range[0, 0].PutValue("Id");
            range[0, 1].PutValue("Name");

            // ملء البيانات باستخدام خاصية Item
            for (int i = 0; i < dt.Rows.Count; i++)
            {
                range[i + 1, 0].PutValue(dt.Rows[i]["Id"]);
                range[i + 1, 1].PutValue(dt.Rows[i]["Name"]);
            }

            // تنسيق صف الرأس باستخدام خاصية Item
            Style style = workbook.CreateStyle();
            style.ForegroundColor = Color.FromArgb(0, 176, 80);
            range[0, 0].SetStyle(style);
            range[0, 1].SetStyle(style);

            // احفظ المصنف
            workbook.Save("RangePropertyItemDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../../cell/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


