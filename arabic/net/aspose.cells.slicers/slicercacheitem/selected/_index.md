---
title: "SlicerCacheItem.Selected"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SlicerCacheItem. تحدد ما إذا كان الـ SlicerCacheItem محددًا أم لا"
type: docs
url: /ar/net/aspose.cells.slicers/slicercacheitem/selected/
---
## SlicerCacheItem.Selected property

تحدد ما إذا كان [`SlicerCacheItem`](../) محددًا أم لا.

```csharp
public bool Selected { get; set; }
```

### ملاحظات

يرجى استخدام طريقة [`SelectItems`](../../slicer/selectitems/) بدلاً من ذلك إذا كنت ترغب في تحديد عنصر. لأن عملية التحديث هذه تسبب أداءً ضعيفًا بسبب إعادة تحميل البيانات بالكامل في كل مرة يتغير فيها التحديد.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCacheItemPropertySelectedDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // إنشاء جدول محوري
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // إضافة مقطع
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "Slicer1");
            Aspose.Cells.Slicers.Slicer slicer = worksheet.Slicers[slicerIndex];
            slicer.StyleType = SlicerStyleType.SlicerStyleLight1;

            // الوصول إلى عناصر ذاكرة التخزين المؤقت للـ slicer
            for (int i = 0; i < slicer.SlicerCache.SlicerCacheItems.Count; i++)
            {
                SlicerCacheItem item = slicer.SlicerCache.SlicerCacheItems[i];
                
                // حدد العنصر الأول، وألغِ تحديد الآخرين
                if (i == 0)
                {
                    item.Selected = true;
                    Console.WriteLine($"Item '{item.Value}' is selected: {item.Selected}");
                }
                else
                {
                    item.Selected = false;
                    Console.WriteLine($"Item '{item.Value}' is selected: {item.Selected}");
                }
            }

            // احفظ المصنف
            workbook.Save("SlicerCacheItemSelectedDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SlicerCacheItem](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


