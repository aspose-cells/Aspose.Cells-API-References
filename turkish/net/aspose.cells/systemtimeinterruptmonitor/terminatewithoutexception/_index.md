---
title: "SystemTimeInterruptMonitor.TerminateWithoutException"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SystemTimeInterruptMonitor özelliği. TerminateWithoutException'a bakın. Bu özellik, bu monitör örneği oluşturulurken kullanıcı tarafından belirtilir."
type: docs
url: /tr/net/aspose.cells/systemtimeinterruptmonitor/terminatewithoutexception/
---
## SystemTimeInterruptMonitor.TerminateWithoutException property

Bakın [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/). Bu özellik, bu monitör örneği oluşturulurken kullanıcı tarafından belirtilir.

```csharp
public override bool TerminateWithoutException { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SystemTimeInterruptMonitorPropertyTerminateWithoutExceptionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // İlk TerminateWithoutException değeriyle SystemTimeInterruptMonitor örneği oluştur.
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);

            // TerminateWithoutException özelliğinin mevcut değerini göster.
            Console.WriteLine("Current TerminateWithoutException value: " + monitor.TerminateWithoutException);

            // 1000 ms zaman sınırlamasıyla izlemeyi başlat.
            monitor.StartMonitor(1000);

            // TerminateWithoutException etkisini, uzun bir işlem denemesiyle göster.
            try
            {
                // Zaman sınırlamasını aşabilecek uzun bir işlemi simüle et.
                for (int i = 0; i < 100000; i++)
                {
                    worksheet.Cells[i, 0].Value = i;
                    if (monitor.IsInterruptionRequested)
                    {
                        Console.WriteLine("Operation interrupted by monitor");
                        break;
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine("Exception caught: " + ex.Message);
            }

            // TerminateWithoutException true olarak ayarlanmış başka bir monitör oluştur.
            SystemTimeInterruptMonitor monitorNoException = new SystemTimeInterruptMonitor(true);
            Console.WriteLine("New monitor TerminateWithoutException value: " + monitorNoException.TerminateWithoutException);

            // Çalışma kitabını kaydedin
            workbook.Save("PropertyTerminateWithoutExceptionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


