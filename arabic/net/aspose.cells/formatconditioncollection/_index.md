---
title: "الفئة FormatConditionCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.FormatConditionCollection. تمثل التنسيق الشرطي. يمكن أن تحتوي FormatConditions على ما يصل إلى ثلاثة تنسيقات شرطية"
type: docs
url: /ar/net/aspose.cells/formatconditioncollection/
---
## FormatConditionCollection class

يمثل تنسيقًا شرطيًا. يمكن أن تحتوي FormatConditions على ما يصل إلى ثلاثة تنسيقات شرطية.

```csharp
public class FormatConditionCollection
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.cells/formatconditioncollection/count/) { get; } | يحصل على عدد الشروط. |
| [Item](../../aspose.cells/formatconditioncollection/item/) { get; } | يحصل على شرط التنسيق حسب الفهرس. |
| [RangeCount](../../aspose.cells/formatconditioncollection/rangecount/) { get; } | يحصل على عدد النطاقات التي تم تنسيقها شرطياً. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.cells/formatconditioncollection/add/)(CellArea, FormatConditionType, OperatorType, string, string) | يضيف شرط تنسيق ونطاق الخلايا المتأثر إلى FormatConditions. يمكن أن تحتوي FormatConditions على ما يصل إلى ثلاثة تنسيقات شرطية. لا يُسمح بالإشارات إلى الأوراق الأخرى في صيغ التنسيق الشرطي. |
| [AddArea](../../aspose.cells/formatconditioncollection/addarea/)(CellArea) | يضيف نطاق خلايا مُنسق شرطياً. |
| [AddCondition](../../aspose.cells/formatconditioncollection/addcondition/#addcondition)(FormatConditionType) | أضف شرط تنسيق. |
| [AddCondition](../../aspose.cells/formatconditioncollection/addcondition/#addcondition_1)(FormatConditionType, OperatorType, string, string) | يضيف شرط تنسيق. |
| [GetCellArea](../../aspose.cells/formatconditioncollection/getcellarea/)(int) | يحصل على نطاق الخلايا المُنسق شرطياً حسب الفهرس. |
| [RemoveArea](../../aspose.cells/formatconditioncollection/removearea/#removearea_1)(int) | يزيل نطاق الخلايا المُنسق شرطياً حسب الفهرس. |
| [RemoveArea](../../aspose.cells/formatconditioncollection/removearea/#removearea)(int, int, int, int) | إزالة التنسيق الشرطي في النطاق. |
| [RemoveCondition](../../aspose.cells/formatconditioncollection/removecondition/)(int) | يزيل شرط التنسيق حسب الفهرس. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionCollectionDemo
    {
        public static void FormatConditionCollectionExample()
        {
            // إنشاء مصنف جديد
            Workbook workbook = new Workbook();

            // احصل على ورقة العمل الأولى
            Worksheet sheet = workbook.Worksheets[0];

            // يضيف تنسيقًا شرطيًا فارغًا
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // يضبط نطاق التنسيق الشرطي
            CellArea ca = new CellArea { StartRow = 0, EndRow = 0, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);
            ca = new CellArea { StartRow = 1, EndRow = 1, StartColumn = 1, EndColumn = 1 };
            fcs.AddArea(ca);

            // يضيف شروط
            int conditionIndex1 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");

            // يضبط لون الخلفية
            FormatCondition fc1 = fcs[conditionIndex1];
            fc1.Style.BackgroundColor = System.Drawing.Color.Red;

            // حفظ ملف Excel
            workbook.Save("FormatConditionCollectionExample.xlsx");
            workbook.Save("FormatConditionCollectionExample.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


