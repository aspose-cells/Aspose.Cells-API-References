---
title: "AbstractInterruptMonitor.IsInterruptionRequested"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AbstractInterruptMonitor. تشير إلى ما إذا كان تم طلب مقاطعة العملية الحالية. إذا كان true فسيتم مقاطعة العملية الحالية. يجب على التنفيذ إجراء فحص سريع وفعال هنا وإلا قد يصبح عنق زجاجة آخر للإجراء"
type: docs
url: /ar/net/aspose.cells/abstractinterruptmonitor/isinterruptionrequested/
---
## AbstractInterruptMonitor.IsInterruptionRequested property

يشير إلى ما إذا كان تم طلب إيقاف العملية الحالية. إذا كان صحيحًا فسيتم إيقاف العملية الحالية. يجب على التنفيذ إجراء فحص سريع وفعال هنا، وإلا قد يصبح عنق زجاجة آخر للإجراء.

```csharp
public abstract bool IsInterruptionRequested { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Threading;
    using System.Threading.Tasks;

    public class AbstractInterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء مراقب مقاطعة وتعيينه إلى دفتر العمل
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;

            // عرض القيمة الأولية
            Console.WriteLine("Initial IsInterruptionRequested: " + monitor.IsInterruptionRequested);

            // ابدأ مهمة الانقطاع
            Task.Run(() =>
            {
                Thread.Sleep(1000); // Wait 1 seconds
                Console.WriteLine("\nTriggering interruption...");
                monitor.Interrupt();
            });

            // محاكاة عملية طويلة الأمد
            Console.WriteLine("Starting data generation...");
            try
            {
                for (int i = 0; i < 500000000; i++)
                {
                    if (monitor.IsInterruptionRequested)
                    {
                        Console.WriteLine($"\nInterrupted at row {i}");
                        break;
                    }

                    worksheet.Cells[i, 0].Value = $"Data {i}";
                    
                    // محاكاة وقت المعالجة
                    if (i % 1000 == 0) 
                        Console.Write(".");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine("\nError: " + ex.Message);
            }

            // حفظ النتيجة
            workbook.Save("InterruptionDemoOutput.xlsx");

            Console.WriteLine("\nWorkbook saved with partial data.");
        }
    }
}
```

### انظر أيضًا

* class [AbstractInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


