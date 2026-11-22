---
title: "AbstractFormulaChangeMonitor.OnCellFormulaChanged"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AbstractFormulaChangeMonitor. الحدث الذي سيتم تشغيله عندما يتم تغيير الصيغة في خلية"
type: docs
url: /ar/net/aspose.cells/abstractformulachangemonitor/oncellformulachanged/
---
## AbstractFormulaChangeMonitor.OnCellFormulaChanged method

الحدث الذي سيتم تشغيله عندما يتم تغيير الصيغة في خلية.

```csharp
public virtual void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetIndex | Int32 | فهرس الورقة للخلية التي تم تغييرها |
| rowIndex | Int32 | فهرس الصف للخلية التي تم تغييرها |
| columnIndex | Int32 | فهرس العمود للخلية التي تم تغييرها |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractFormulaChangeMonitorMethodOnCellFormulaChangedWithInt32Int32Int32Demo : AbstractFormulaChangeMonitor
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أنشئ مثيلاً لفئتنا التجريبية التي ترث من AbstractFormulaChangeMonitor
            var monitor = new AbstractFormulaChangeMonitorMethodOnCellFormulaChangedWithInt32Int32Int32Demo();

            // ضع صيغة ما في خلية لتفعيل التغيير
            worksheet.Cells["A1"].Formula = "=SUM(B1:B10)";

            try
            {
                // استدعِ OnCellFormulaChanged مع فهرس الورقة 0، الصف 0، العمود 0 (A1)
                monitor.OnCellFormulaChanged(0, 0, 0);

                Console.WriteLine("OnCellFormulaChanged called successfully for cell A1");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing OnCellFormulaChanged method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("OnCellFormulaChangedDemo.xlsx");
        }

        public override void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
        {
            // تنفيذ لمعالجة تغيير الصيغة
            Console.WriteLine($"Formula changed in sheet {sheetIndex} at row {rowIndex}, column {columnIndex}");
        }

    }
}
```

### انظر أيضًا

* class [AbstractFormulaChangeMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


