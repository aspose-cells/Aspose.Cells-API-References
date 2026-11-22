---
title: "InterruptMonitor.IsInterruptionRequested"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية InterruptMonitor. وضع علامة على المراقب بأنه يطلب مقاطعة"
type: docs
url: /ar/net/aspose.cells/interruptmonitor/isinterruptionrequested/
---
## InterruptMonitor.IsInterruptionRequested property

وضع علامة على المراقب بأنه يطلب المقاطعة

```csharp
public override bool IsInterruptionRequested { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class InterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد والوصول إلى ورقة العمل الأولى الخاصة به
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء مراقب مقاطعة وتعيينه إلى دفتر العمل
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;

            // عرض الحالة الأولية لـ IsInterruptionRequested
            Console.WriteLine("Initial IsInterruptionRequested value: " + monitor.IsInterruptionRequested);

            // محاكاة عملية معالجة بيانات طويلة الأمد
            Console.WriteLine("Starting data processing...");
            for (int rowIdx = 0; rowIdx < 10000; rowIdx++)
            {
                // طلب مقاطعة بعد معالجة 500 صف
                if (rowIdx == 500)
                {
                    monitor.Interrupt();
                    Console.WriteLine("Interrupt requested. IsInterruptionRequested: " + monitor.IsInterruptionRequested);
                }

                // التحقق من طلب المقاطعة
                if (monitor.IsInterruptionRequested)
                {
                    Console.WriteLine($"Processing interrupted at row {rowIdx}");
                    break;
                }

                // محاكاة معالجة البيانات
                worksheet.Cells[rowIdx, 0].Value = $"Row {rowIdx} data";
            }

            // احفظ المصنف المعدل
            workbook.Save("InterruptionDemoOutput.xlsx");
            Console.WriteLine("File saved with partial data due to interruption.");
        }
    }
}
```

### انظر أيضًا

* class [InterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


