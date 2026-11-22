---
title: "DeleteOptions.FormulaChangeMonitor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DeleteOptions. تحصل/تضبط المراقب لتتبع التغييرات الناجمة عن الحذف"
type: docs
url: /ar/net/aspose.cells/deleteoptions/formulachangemonitor/
---
## DeleteOptions.FormulaChangeMonitor property

يحصل على/يضبط المراقب لتتبع التغييرات الناجمة عن الحذف.

```csharp
public AbstractFormulaChangeMonitor FormulaChangeMonitor { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteOptionsPropertyFormulaChangeMonitorDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // إعداد بيانات الاختبار
            cells["A1"].Formula = "=A5";
            cells["A5"].Value = 10;
            
            // إضافة تنسيق شرطي
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            fcc.Add(CellArea.CreateCellArea(0, 3, 1, 4), FormatConditionType.Expression,
                OperatorType.Equal, "=A8>0", "");

            // إنشاء وتعيين المراقب
            CustomFormulaChangeMonitor monitor = new CustomFormulaChangeMonitor();
            DeleteOptions options = new DeleteOptions
            {
                FormulaChangeMonitor = monitor,
                UpdateReference = true
            };

            // حذف الصف الذي يجب أن يسبب تغييرات في الصيغ
            cells.DeleteRows(2, 1, options);

            // إخراج نتائج المراقبة
            Console.WriteLine("Cell formula changes detected: " + monitor.CellChangesDetected);
            Console.WriteLine("Format condition changes detected: " + monitor.FormatConditionChangesDetected);
        }
    }

    public class CustomFormulaChangeMonitor : AbstractFormulaChangeMonitor
    {
        public bool CellChangesDetected { get; private set; }
        public bool FormatConditionChangesDetected { get; private set; }

        public override void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
        {
            CellChangesDetected = true;
            Console.WriteLine($"Cell formula changed at Sheet {sheetIndex}, Row {rowIndex}, Column {columnIndex}");
        }

        public override void OnFormatConditionFormulaChanged(FormatCondition fc)
        {
            FormatConditionChangesDetected = true;
            Console.WriteLine("Format condition formula changed");
        }
    }
}
```

### انظر أيضًا

* class [AbstractFormulaChangeMonitor](../../abstractformulachangemonitor/)
* class [DeleteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


