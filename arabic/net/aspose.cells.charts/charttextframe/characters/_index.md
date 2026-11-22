---
title: "ChartTextFrame.Characters"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ChartTextFrame. تُرجع كائن Characters يمثل نطاقًا من الأحرف داخل النص"
type: docs
url: /ar/net/aspose.cells.charts/charttextframe/characters/
---
## ChartTextFrame.Characters method

يرجع كائن Characters الذي يمثل نطاقًا من الأحرف داخل النص.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startIndex | Int32 | فهرس بداية الحرف. |
| الطول | Int32 | عدد الأحرف. |

### قيمة الإرجاع

كائن الأحرف.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFrameMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // إنشاء مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // الوصول إلى تسميات البيانات وتعيين حجم الخط للأحرف المحددة
            chart.NSeries[0].Points[0].DataLabels.ShowValue = true;
            chart.NSeries[0].Points[0].DataLabels.Characters(0, 5).Font.Size = 14;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


