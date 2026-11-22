---
title: "فئة DataBar"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.DataBar فئة. تصف قاعدة تنسيق الشرط للـ DataBar. تعرض قاعدة تنسيق الشرط هذه شريط بيانات متدرج في نطاق الخلايا"
type: docs
url: /ar/net/aspose.cells/databar/
---
## DataBar class

وصف قاعدة تنسيق الخلايا الشرطي DataBar. هذه القاعدة تعرض شريط بيانات متدرج في نطاق الخلايا.

```csharp
public class DataBar
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AxisColor](../../aspose.cells/databar/axiscolor/) { get; set; } | يحصل على لون المحور للخلايا التي تم تنسيقها شرطياً كشريط بيانات. |
| [AxisPosition](../../aspose.cells/databar/axisposition/) { get; set; } | يحصل أو يضبط موضع محور أشرطة البيانات المحددة بواسطة قاعدة تنسيق شرطي. |
| [BarBorder](../../aspose.cells/databar/barborder/) { get; } | يحصل على كائن يحدد حد شريط البيانات. |
| [BarFillType](../../aspose.cells/databar/barfilltype/) { get; set; } | يحصل أو يضبط طريقة ملء شريط البيانات باللون. |
| [Color](../../aspose.cells/databar/color/) { get; set; } | احصل أو اضبط لون شريط البيانات هذا. |
| [Direction](../../aspose.cells/databar/direction/) { get; set; } | يحصل أو يضبط الاتجاه الذي يُعرض به شريط البيانات. |
| [MaxCfvo](../../aspose.cells/databar/maxcfvo/) { get; } | احصل أو اضبط كائن القيمة القصوى لهذا شريط البيانات. لا يمكن تعيين null أو CFValueObject من النوع FormatConditionValueType.Min إليه. |
| [MaxLength](../../aspose.cells/databar/maxlength/) { get; set; } | يمثل الحد الأقصى لطول شريط البيانات. |
| [MinCfvo](../../aspose.cells/databar/mincfvo/) { get; } | احصل أو اضبط كائن القيمة الدنيا لهذا شريط البيانات. لا يمكن تعيين null أو CFValueObject من النوع FormatConditionValueType.Max إليه. |
| [MinLength](../../aspose.cells/databar/minlength/) { get; set; } | يمثل الحد الأدنى لطول شريط البيانات. |
| [NegativeBarFormat](../../aspose.cells/databar/negativebarformat/) { get; } | يحصل على كائن NegativeBarFormat المرتبط بقاعدة تنسيق شرطي لشريط البيانات. |
| [ShowValue](../../aspose.cells/databar/showvalue/) { get; set; } | احصل أو اضبط العلامة التي تشير إلى ما إذا كان يجب إظهار قيم الخلايا التي يُطبق عليها شريط البيانات هذا. القيمة الافتراضية هي true. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [ToImage](../../aspose.cells/databar/toimage/)(Cell, ImageOrPrintOptions) | قم بتحويل شريط البيانات في الخلية إلى مصفوفة بايت للصورة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarDemo
    {
        public static void DataBarExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // يضيف تنسيقًا شرطيًا فارغًا
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // يضبط نطاق التنسيق الشرطي
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // يضيف شرطًا
            int idx = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = fcs[idx];

            // احصل على شريط البيانات
            DataBar dataBar = cond.DataBar;

            // اضبط خصائص شريط البيانات
            dataBar.Color = Color.Orange;
            dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MinCfvo.Value = 30;
            dataBar.ShowValue = false;
            dataBar.BarBorder.Type = DataBarBorderType.Solid;
            dataBar.BarBorder.Color = Color.Plum;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint;
            dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.Color = Color.White;
            dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // ضع قيم الخلايا
            Aspose.Cells.Cell cell1 = sheet.Cells["A1"];
            cell1.PutValue(10);
            Aspose.Cells.Cell cell2 = sheet.Cells["A2"];
            cell2.PutValue(120);
            Aspose.Cells.Cell cell3 = sheet.Cells["A3"];
            cell3.PutValue(260);

            // حفظ ملف Excel
            workbook.Save("DataBarExample.xlsx");
            workbook.Save("DataBarExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


