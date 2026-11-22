---
title: "Top10Filter.Items"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Top10Filter. تحصل وتضبط القيمة العليا أو السفلى لاستخدامها كمعيار للفلتر"
type: docs
url: /ar/net/aspose.cells/top10filter/items/
---
## Top10Filter.Items property

يحصل ويعيّن القيمة العليا أو السفلى لاستخدامها كمعيار للفلتر.

```csharp
public int Items { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class Top10FilterPropertyItemsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["A5"].PutValue("Grapes");
            worksheet.Cells["A6"].PutValue("Mango");
            
            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:A6", "C1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // تطبيق فلتر أعلى 10
            pivotTable.BaseFields[0].FilterTop10(0, PivotFilterType.Count, false, 2);
            
            // احصل على الفلتر وأظهر خاصية Items
            PivotFilter filter = pivotTable.BaseFields[0].GetFilters()[0];
            int itemsCount = filter.GetTop10Value().Items;
            
            Console.WriteLine("Top 10 Filter Items Count: " + itemsCount);
        }
    }
}
```

### انظر أيضًا

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


