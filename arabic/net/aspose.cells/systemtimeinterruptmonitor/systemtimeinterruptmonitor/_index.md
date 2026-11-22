---
title: "SystemTimeInterruptMonitor.SystemTimeInterruptMonitor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ SystemTimeInterruptMonitor. ينشئ مراقب مقاطعة واحد"
type: docs
url: /ar/net/aspose.cells/systemtimeinterruptmonitor/systemtimeinterruptmonitor/
---
## SystemTimeInterruptMonitor constructor

ينشئ مراقب انقطاع واحد.

```csharp
public SystemTimeInterruptMonitor(bool terminateWithoutException)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| terminateWithoutException | Boolean | [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/) |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SystemTimeInterruptMonitorMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // إنشاء نسخة مع تعيين terminateWithoutException إلى false
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);

            // إعداد خيارات التحميل مع المراقب
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // بدء المراقبة بحد زمني قدره ثانية واحدة
            monitor.StartMonitor(1000);

            try
            {
                // محاولة تحميل دفتر عمل
                Workbook wb = new Workbook("sample.xlsx", lopts);

                // إعادة ضبط المراقب لعملية الحفظ بحد 1.5 ثانية
                monitor.StartMonitor(1500);
                wb.Save("output.xlsx");
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

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


