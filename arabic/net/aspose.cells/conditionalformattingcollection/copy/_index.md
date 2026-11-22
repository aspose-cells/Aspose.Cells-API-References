---
title: "ConditionalFormattingCollection.Copy"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ConditionalFormattingCollection. تنسخ التنسيق الشرطي"
type: docs
url: /ar/net/aspose.cells/conditionalformattingcollection/copy/
---
## ConditionalFormattingCollection.Copy method

ينسخ التنسيق الشرطي.

```csharp
public void Copy(ConditionalFormattingCollection cfs)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cfs | ConditionalFormattingCollection | التنسيق الشرطي |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingCollectionMethodCopyWithConditionalFormattingCollectioDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];

            // إنشاء مصنف مصدر مع تنسيق شرطي
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];

            // إضافة تنسيق شرطي نموذجي إلى ورقة المصدر
            int index = sourceSheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sourceSheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            
            // إنشاء وتطبيق نمط على شرط التنسيق
            Style style = sourceWorkbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.Red;
            FormatCondition fc = fcc[0];
            fc.Style = style;

            // تطبيق على نطاق
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 5;
            area.StartColumn = 0;
            area.EndColumn = 5;
            fcc.AddArea(area);

            // نسخ التنسيق الشرطي من المصدر إلى الوجهة
            destSheet.ConditionalFormattings.Copy(sourceSheet.ConditionalFormattings);

            // احفظ المصنف
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


