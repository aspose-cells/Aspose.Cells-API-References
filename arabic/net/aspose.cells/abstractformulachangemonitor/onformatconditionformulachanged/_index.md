---
title: "AbstractFormulaChangeMonitor.OnFormatConditionFormulaChanged"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AbstractFormulaChangeMonitor. الحدث الذي سيتم تشغيله عندما يتم تغيير صيغة FormatCondition"
type: docs
url: /ar/net/aspose.cells/abstractformulachangemonitor/onformatconditionformulachanged/
---
## AbstractFormulaChangeMonitor.OnFormatConditionFormulaChanged method

الحدث الذي سيتم تشغيله عندما يتم تغيير صيغة FormatCondition.

```csharp
public virtual void OnFormatConditionFormulaChanged(FormatCondition fc)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fc | FormatCondition | كائن FormatCondition الذي تم تغيير صيغته |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractFormulaChangeMonitorMethodOnFormatConditionFormulaChangedWithFormatConditionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // أنشئ تنسيقًا شرطيًا
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // أنشئ شرط تنسيق
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style = workbook.CreateStyle();
            fc.Style.Font.Color = System.Drawing.Color.Red;

            // أنشئ مراقبًا مخصصًا
            var monitor = new CustomFormulaChangeMonitor();

            try
            {
                // استدعِ طريقة OnFormatConditionFormulaChanged
                monitor.OnFormatConditionFormulaChanged(fc);

                Console.WriteLine("Method executed successfully with FormatCondition parameter");

                // تطبيق التنسيق الشرطي على نطاق
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 2;
                area.EndColumn = 0;
                fcs.AddArea(area);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing OnFormatConditionFormulaChanged method: {ex.Message}");
            }

            workbook.Save("MethodOnFormatConditionFormulaChangedDemo.xlsx");
        }
    }

    public class CustomFormulaChangeMonitor : AbstractFormulaChangeMonitor
    {
        public override void OnFormatConditionFormulaChanged(FormatCondition fc)
        {
            Console.WriteLine($"Format condition formula changed. Type: {fc.Type}, Formula1: {fc.Formula1}, Formula2: {fc.Formula2}");
        }
    }

}
```

### انظر أيضًا

* class [FormatCondition](../../formatcondition/)
* class [AbstractFormulaChangeMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


