---
title: "الفئة SystemTimeInterruptMonitor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.SystemTimeInterruptMonitor. تنفيذ بسيط لـ AbstractInterruptMonitor عن طريق فحص ومقارنة الوقت النظامي الحالي مع الحد المحدد من قبل المستخدم"
type: docs
url: /ar/net/aspose.cells/systemtimeinterruptmonitor/
---
## SystemTimeInterruptMonitor class

تنفيذ بسيط لـ [`AbstractInterruptMonitor`](../abstractinterruptmonitor/) عن طريق فحص ومقارنة الوقت النظامي الحالي مع الحد المحدد من قبل المستخدم.

```csharp
public class SystemTimeInterruptMonitor : AbstractInterruptMonitor
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [SystemTimeInterruptMonitor](systemtimeinterruptmonitor/)(bool) | ينشئ مراقب انقطاع واحد. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/systemtimeinterruptmonitor/isinterruptionrequested/) { get; } | يتحقق هذا التنفيذ فقط مما إذا كانت تكلفة الوقت (من لحظة بدء هذا المراقب حتى الآن) أكبر من الحد المحدد من قبل المستخدم. |
| override [TerminateWithoutException](../../aspose.cells/systemtimeinterruptmonitor/terminatewithoutexception/) { get; } | انظر إلى [`TerminateWithoutException`](../abstractinterruptmonitor/terminatewithoutexception/). يتم تحديد هذه الخاصية من قبل المستخدم عند إنشاء مثيل هذا المراقب. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [StartMonitor](../../aspose.cells/systemtimeinterruptmonitor/startmonitor/)(int) | يبدأ المراقب بالحد الزمني المحدد. وقت البدء لحساب تكلفة الوقت هو لحظة استدعاء هذه الطريقة، لذا يجب بدء الإجراء الذي يحتاج إلى مراقبة مباشرةً بعد هذا الاستدعاء. |

### ملاحظات

هذا التنفيذ هو مجرد حل بسيط للسيناريوهات البسيطة. يحتاج إلى استرجاع وفحص الوقت النظامي بشكل متكرر، لذا قد يؤثر سلبًا على الأداء إلى حد ما.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SystemTimeInterruptMonitorDemo
    {
        public static void SystemTimeInterruptMonitorExample()
        {
            // إنشاء مثيل من SystemTimeInterruptMonitor مع تعيين terminateWithoutException إلى false
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);

            // إنشاء LoadOptions وتعيين InterruptMonitor إلى المراقب المُنشأ
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // بدء المراقبة بحد زمني قدره 1000 مللي ثانية (1 ثانية)
            monitor.StartMonitor(1000);

            try
            {
                // تحميل مصنف باستخدام LoadOptions المحددة
                Workbook wb = new Workbook("Large.xlsx", lopts);

                // إذا تجاوز الوقت المستغرق في تحميل ملف القالب ثانية واحدة، سيتطلب التوقف وسيتم إلقاء الاستثناء هنا
                // إلا، ابدأ بمراقبة عملية الحفظ بحد زمني جديد
                monitor.StartMonitor(1500); // time limit is 1.5 seconds

                // احفظ المصنف
                wb.Save("SystemTimeInterruptMonitorExample.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Operation interrupted: " + ex.Message);
            }
        }
    }
}
```

### انظر أيضًا

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


