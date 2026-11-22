---
title: "الفئة ThreadInterruptMonitor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.ThreadInterruptMonitor. تنفيذ بسيط لـ AbstractInterruptMonitor عن طريق بدء خيط آخر لتطلب المقاطعة بعد النوم للحد المحدد من قبل المستخدم"
type: docs
url: /ar/net/aspose.cells/threadinterruptmonitor/
---
## ThreadInterruptMonitor class

تنفيذ بسيط لـ [`AbstractInterruptMonitor`](../abstractinterruptmonitor/) عن طريق بدء خيط آخر لتطلب المقاطعة بعد النوم للحد المحدد من قبل المستخدم.

```csharp
public class ThreadInterruptMonitor : AbstractInterruptMonitor
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [ThreadInterruptMonitor](threadinterruptmonitor/)(bool) | ينشئ مراقب انقطاع واحد. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/threadinterruptmonitor/isinterruptionrequested/) { get; } | يتحقق هذا التنفيذ فقط مما إذا كانت تكلفة الوقت (من لحظة بدء هذا المراقب حتى الآن) أكبر من الحد المحدد من قبل المستخدم. |
| override [TerminateWithoutException](../../aspose.cells/threadinterruptmonitor/terminatewithoutexception/) { get; } | انظر إلى [`TerminateWithoutException`](../abstractinterruptmonitor/terminatewithoutexception/). يتم تحديد هذه الخاصية من قبل المستخدم عند إنشاء مثيل هذا المراقب. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [FinishMonitor](../../aspose.cells/threadinterruptmonitor/finishmonitor/)() | ينهي المراقب لإجراء واحد. |
| [StartMonitor](../../aspose.cells/threadinterruptmonitor/startmonitor/)(int) | يبدأ المراقب بالحد الزمني المحدد. وقت البدء لحساب تكلفة الوقت هو لحظة استدعاء هذه الطريقة، لذا يجب بدء الإجراء الذي يحتاج إلى مراقبة مباشرةً بعد هذا الاستدعاء. |

### ملاحظات

يمكن استخدام نسخة واحدة من المراقب بشكل متكرر، طالما أنك تراقب كل عملية بالتسلسل. لا ينبغي استخدامها لمراقبة إجراءات متعددة في وقت واحد عبر خيوط متعددة.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadInterruptMonitorDemo
    {
        public static void ThreadInterruptMonitorExample()
        {
            // إنشاء نسخة من ThreadInterruptMonitor مع تعيين terminateWithoutException إلى false
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);

            // إنشاء LoadOptions وتعيين InterruptMonitor إلى المراقب المُنشأ
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // ابدأ المراقب بحد زمني قدره 1000 مللي ثانية (1 ثانية)
            monitor.StartMonitor(1000);

            try
            {
                // تحميل مصنف باستخدام LoadOptions المحددة
                Workbook wb = new Workbook("Large.xlsx", lopts);

                // أنهِ المراقب لإجراء التحميل
                monitor.FinishMonitor();

                // ابدأ المراقب مرة أخرى بحد زمني جديد قدره 1500 مللي ثانية (1.5 ثانية)
                monitor.StartMonitor(1500);

                // احفظ المصنف
                wb.Save("result.xlsx");

                // أنهِ المراقب لإجراء الحفظ
                monitor.FinishMonitor();
            }
            catch (Exception ex)
            {
                Console.WriteLine("An exception occurred: " + ex.Message);
            }
        }
    }
}
```

### انظر أيضًا

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


