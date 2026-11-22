---
title: "الفئة InterruptMonitor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.InterruptMonitor. تمثل جميع العمليات المتعلقة بالمقاطعة"
type: docs
url: /ar/net/aspose.cells/interruptmonitor/
---
## InterruptMonitor class

يمثل جميع العمليات المتعلقة بالمقاطعة.

```csharp
public class InterruptMonitor : AbstractInterruptMonitor
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [InterruptMonitor](interruptmonitor/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/interruptmonitor/isinterruptionrequested/) { get; } | وضع علامة على المراقب بأنه يطلب المقاطعة |
| virtual [TerminateWithoutException](../../aspose.cells/abstractinterruptmonitor/terminatewithoutexception/) { get; } | عند مقاطعة الإجراء، ما إذا كان سيتم إنهاء الإجراء بهدوء أو رمي استثناء. القيمة الافتراضية هي false، أي عندما يكون [`IsInterruptionRequested`](../abstractinterruptmonitor/isinterruptionrequested/) true، سيتم رمي [`CellsException`](../cellsexception/) بالرمز Interrupted. (موروث من [`AbstractInterruptMonitor`](../abstractinterruptmonitor/).) |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Interrupt](../../aspose.cells/interruptmonitor/interrupt/)() | مقاطعة المشغل الحالي. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassInterruptMonitorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف بعض البيانات التجريبية
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // إنشاء وتعيين مراقب المقاطعة
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;
            
            try
            {
                Console.WriteLine("Starting save operation...");
                
                // محاكاة مقاطعة العملية
                monitor.Interrupt();
                
                // محاولة الحفظ (يجب أن يتم مقاطعته)
                workbook.Save("output.pdf", SaveFormat.Pdf);
                Console.WriteLine("Save completed successfully.");
            }
            catch (CellsException e)
            {
                if (e.Code == ExceptionType.Interrupted)
                {
                    Console.WriteLine("Operation was successfully interrupted.");
                }
                else
                {
                    Console.WriteLine("Error occurred: " + e.Message);
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


