---
title: "Cells.FirstCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cells. يحصل على أول خلية في ورقة العمل هذه"
type: docs
url: /ar/net/aspose.cells/cells/firstcell/
---
## Cells.FirstCell property

يحصل على الخلية الأولى في ورقة العمل هذه.

```csharp
public Cell FirstCell { get; }
```

### ملاحظات

يعيد null إذا لم توجد بيانات في ورقة العمل.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class CellsPropertyFirstCellDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B3"].PutValue(2000);
            
            // احصل على مجموعة الخلايا
            Cells cells = worksheet.Cells;
            
            // عرض خاصية FirstCell
            Cell firstCell = cells.FirstCell;
            Console.WriteLine($"First cell address: {firstCell.Name}");
            Console.WriteLine($"First cell value: {firstCell.Value}");
            
            // إنشاء مخطط باستخدام FirstCell و LastCell
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange($"{cells.FirstCell.Name}:{cells.LastCell.Name}", true);
            chart.ShowLegend = true;
            
            // احفظ المصنف
            workbook.Save("FirstCellDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


