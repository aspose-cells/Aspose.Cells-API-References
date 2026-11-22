---
title: "AutoFilter.SetRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AutoFilter. يحدد النطاق الذي ينطبق عليه AutoFilter المحدد"
type: docs
url: /ar/net/aspose.cells/autofilter/setrange/
---
## AutoFilter.SetRange method

يحدد النطاق الذي ينطبق عليه AutoFilter المحدد.

```csharp
public void SetRange(int row, int startColumn, int endColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف. |
| startColumn | Int32 | فهرس العمود الابتدائي. |
| endColumn | Int32 | فهرس عمود النهاية. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodSetRangeWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("Header");
            sheet.Cells["A2"].PutValue("Data1");
            sheet.Cells["A3"].PutValue("Data2");
            sheet.Cells["A4"].PutValue("Data3");

            // تحديد نطاق الفلتر التلقائي (firstRow, firstColumn, totalRows)
            sheet.AutoFilter.SetRange(0, 0, 4);

            // تطبيق الفلتر
            sheet.AutoFilter.Custom(0, FilterOperatorType.Equal, "Data2");

            // تحديث الفلتر
            sheet.AutoFilter.Refresh();

            // احفظ المصنف
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


