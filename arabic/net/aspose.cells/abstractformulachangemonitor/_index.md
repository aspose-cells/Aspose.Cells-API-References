---
title: "الفئة AbstractFormulaChangeMonitor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.AbstractFormulaChangeMonitor. مراقب للمستخدم لتتبع تغير الصيغ أثناء عمليات معينة"
type: docs
url: /ar/net/aspose.cells/abstractformulachangemonitor/
---
## AbstractFormulaChangeMonitor class

مراقبة للمستخدم لتتبع تغير الصيغ أثناء عمليات معينة.

```csharp
public abstract class AbstractFormulaChangeMonitor
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| virtual [OnCellFormulaChanged](../../aspose.cells/abstractformulachangemonitor/oncellformulachanged/)(int, int, int) | الحدث الذي سيتم تشغيله عندما يتم تغيير الصيغة في خلية. |
| virtual [OnFormatConditionFormulaChanged](../../aspose.cells/abstractformulachangemonitor/onformatconditionformulachanged/)(FormatCondition) | الحدث الذي سيتم تشغيله عندما يتم تغيير صيغة FormatCondition. |

### ملاحظات

على سبيل المثال، أثناء حذف/إدراج نطاق من الخلايا، قد تتغير صيغ الخلايا الأخرى بسبب إزاحة المراجع. يرجى ملاحظة أن طرق المراقب قد تُستدعى عدة مرات لكائن واحد يحتوي على الصيغة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassAbstractFormulaChangeMonitorDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            
            // ضبط بعض الصيغ في الخلايا
            worksheet.Cells["A1"].Formula = "=B1+C1";
            worksheet.Cells["B1"].Formula = "=D1*2";
            worksheet.Cells["C1"].Value = 5;
            worksheet.Cells["D1"].Value = 10;

            InsertOptions options = new InsertOptions();
            options.FormulaChangeMonitor = new MyFormulaChangeMonitor(wb.Worksheets);
            
            // إدراج صفوف ستؤدي إلى تغيير الصيغ
            worksheet.Cells.InsertRows(0, 2, options);
        }
    }

    public class MyFormulaChangeMonitor : AbstractFormulaChangeMonitor
    {
        private readonly WorksheetCollection mWorksheets;
        
        public MyFormulaChangeMonitor(WorksheetCollection worksheets)
        {
            mWorksheets = worksheets;
        }

        public override void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
        {
            Console.WriteLine($"Formula changed in {mWorksheets[sheetIndex].Name}!{CellsHelper.CellIndexToName(rowIndex, columnIndex)}");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


