---
title: "PivotField.Position"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotField. تمثل فهرس PivotField في المنطقة"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/position/
---
## PivotField.Position property

تمثل فهرس [`PivotField`](../) في المنطقة.

```csharp
public int Position { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyPositionDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر
            Workbook wb = new Workbook("NET46429_a.xlsx");
            
            // الوصول إلى الورقة الأولى وجدولها المحوري
            Worksheet ws = wb.Worksheets[0];
            PivotTable pt = ws.PivotTables[0];
            
            // عرض استخدام خاصية Position
            int position = pt.PageFields[0].Position;
            Console.WriteLine("Position of first page field: " + position);
            
            // استخدم position لعرض صفحات مرشح التقرير
            pt.ShowReportFilterPageByIndex(position);
            
            // احفظ المصنف
            wb.Save("PivotFieldPropertyPositionDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


