---
title: "AbstractInterruptMonitor.TerminateWithoutException"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AbstractInterruptMonitor. عندما يتم مقاطعة الإجراء هل يتم إنهاؤه بهدوء أم رمي استثناء. القيمة الافتراضية هي false أي عندما يكون IsInterruptionRequested true سيتم رمي CellsException بالرمز Interrupted."
type: docs
url: /ar/net/aspose.cells/abstractinterruptmonitor/terminatewithoutexception/
---
## AbstractInterruptMonitor.TerminateWithoutException property

عند مقاطعة الإجراء، هل يتم إنهاؤه بهدوء أم رمي استثناء. القيمة الافتراضية هي false، أي عندما يكون [`IsInterruptionRequested`](../isinterruptionrequested/) true، سيتم رمي [`CellsException`](../../cellsexception/) بالرمز Interrupted.

```csharp
public virtual bool TerminateWithoutException { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractInterruptMonitorPropertyTerminateWithoutExceptionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // املأ ورقة العمل لإنشاء عبء معالجة
            for (int row = 0; row < 5000; row++)
            {
                for (int col = 0; col < 50; col++)
                {
                    worksheet.Cells[row, col].Value = "SampleData";
                }
            }

            // عرض SystemTimeInterruptMonitor مع إنهاء بالاستثناء
            var interruptMonitor1 = new SystemTimeInterruptMonitor(terminateWithoutException: false);
            Console.WriteLine($"Initial TerminateWithoutException: {interruptMonitor1.TerminateWithoutException}");

            workbook.InterruptMonitor = interruptMonitor1;
            interruptMonitor1.StartMonitor(1); // Set 1ms timeout

            try
            {
                workbook.Save("TerminateWithException.xlsx");
                Console.WriteLine("Saved successfully (unexpected with false setting)");
            }
            catch (CellsException ex)
            {
                Console.WriteLine($"Operation terminated with exception: {ex.Message}");
            }

            // عرض SystemTimeInterruptMonitor مع إنهاء صامت
            var interruptMonitor2 = new SystemTimeInterruptMonitor(terminateWithoutException: true);
            Console.WriteLine($"\nNew TerminateWithoutException: {interruptMonitor2.TerminateWithoutException}");

            workbook.InterruptMonitor = interruptMonitor2;
            interruptMonitor2.StartMonitor(1);

            try
            {
                workbook.Save("TerminateSilently.xlsx");
                Console.WriteLine("Saved without exception (expected with true setting)");
            }
            catch (CellsException)
            {
                Console.WriteLine("Exception caught (unexpected with true setting)");
            }

        }
    }

}
```

### انظر أيضًا

* class [AbstractInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


