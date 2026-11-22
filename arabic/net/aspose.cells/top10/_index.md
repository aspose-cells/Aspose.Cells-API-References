---
title: "الفئة Top10"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Top10. صِف قاعدة التنسيق الشرطي Top10. تُبرز هذه القاعدة الخلايا التي تقع قيمها في الفئة العليا N أو الفئة السفلى N كما هو محدد"
type: docs
url: /ar/net/aspose.cells/top10/
---
## Top10 class

وصف قاعدة التنسيق الشرطي Top10. تُبرز قاعدة التنسيق الشرطي هذه الخلايا التي تقع قيمها في الفئة العليا N أو الفئة السفلى N، كما هو محدد.

```csharp
public class Top10
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [Top10](top10/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [IsBottom](../../aspose.cells/top10/isbottom/) { get; set; } | احصل أو عيّن ما إذا كانت قاعدة "top/bottom n" هي قاعدة "bottom n". القيمة الافتراضية هي false. |
| [IsPercent](../../aspose.cells/top10/ispercent/) { get; set; } | احصل أو عيّن ما إذا كانت قاعدة "top/bottom n" هي قاعدة "top/bottom n percent". القيمة الافتراضية هي false. |
| [Rank](../../aspose.cells/top10/rank/) { get; set; } | احصل أو عيّن قيمة "n" في قاعدة التنسيق الشرطي "top/bottom n". إذا كان IsPercent صحيحًا، يجب أن تكون القيمة بين 0 و 100. وإلا يجب أن تكون بين 0 و 1000. القيمة الافتراضية هي 10. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class Top10Demo
    {
        public static void Top10Example()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // يضيف تنسيقًا شرطيًا فارغًا
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // يضبط نطاق التنسيق الشرطي
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // يضيف شرطًا
            int conditionIndex = fcs.AddCondition(FormatConditionType.Top10);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            // ضبط الخصائص
            Top10 top10 = fc.Top10;
            top10.IsPercent = false;
            top10.IsBottom = false;
            top10.Rank = 5;

            // حفظ ملف Excel
            workbook.Save("Top10Example.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


