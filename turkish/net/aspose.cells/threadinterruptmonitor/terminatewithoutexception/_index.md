---
title: "ThreadInterruptMonitor.TerminateWithoutException"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreadInterruptMonitor özelliği. TerminateWithoutException'a bakın. Bu özellik, izleyici örneği oluşturulurken kullanıcı tarafından belirtilir"
type: docs
url: /tr/net/aspose.cells/threadinterruptmonitor/terminatewithoutexception/
---
## ThreadInterruptMonitor.TerminateWithoutException property

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

    public class ThreadInterruptMonitorPropertyTerminateWithoutExceptionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // İlk TerminateWithoutException değeriyle ThreadInterruptMonitor örneği oluşturun
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
            
            // Özelliğin mevcut değerini görüntüleyin
            Console.WriteLine("Current TerminateWithoutException value: " + monitor.TerminateWithoutException);

            // 5 saniyelik bir sınırla izlemeyi başlatın
            monitor.StartMonitor(5000);

            // Kesintiye uğrayabilecek işlemi göster
            try
            {
                for (int i = 0; i < 100000; i++)
                {
                    // Uzun işleme simüle et
                    if (monitor.IsInterruptionRequested)
                    {
                        Console.WriteLine("Processing was interrupted");
                        break;
                    }
                    worksheet.Cells[i, 0].Value = "Value " + i;
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine("Exception occurred: " + ex.Message);
            }
            finally
            {
                monitor.FinishMonitor();
            }

            // TerminateWithoutException true olarak ayarlanmış başka bir monitör oluştur.
            ThreadInterruptMonitor silentMonitor = new ThreadInterruptMonitor(true);
            Console.WriteLine("\nNew monitor TerminateWithoutException value: " + silentMonitor.TerminateWithoutException);

            // Sonucu kaydet
            workbook.Save("PropertyTerminateWithoutExceptionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


