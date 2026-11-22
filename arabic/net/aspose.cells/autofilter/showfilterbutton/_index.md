---
title: "AutoFilter.ShowFilterButton"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AutoFilter. تشير إلى ما إذا كان زر AutoFilter لهذا العمود مرئيًا"
type: docs
url: /ar/net/aspose.cells/autofilter/showfilterbutton/
---
## AutoFilter.ShowFilterButton property

يشير إلى ما إذا كان زر AutoFilter لهذا العمود مرئيًا.

```csharp
public bool ShowFilterButton { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertyShowFilterButtonDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // إنشاء كائن/جدول قائمة
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];

            // تمكين autofilter وعرض أزرار الفلتر
            table.AutoFilter.ShowFilterButton = true;

            // احفظ المصنف
            workbook.Save("output_with_filter_buttons.xlsx");

            // إخفاء أزرار الفلتر
            table.AutoFilter.ShowFilterButton = false;
            workbook.Save("output_without_filter_buttons.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


