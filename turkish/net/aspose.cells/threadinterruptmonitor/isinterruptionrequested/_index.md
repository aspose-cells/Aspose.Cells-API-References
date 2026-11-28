---
title: "ThreadInterruptMonitor.IsInterruptionRequested"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreadInterruptMonitor özelliği. Bu uygulama, bu izleyiciyi başlatma zamanından şu ana kadar geçen sürenin kullanıcı tarafından belirlenen sınırı aşıp aşmadığını kontrol eder"
type: docs
url: /tr/net/aspose.cells/threadinterruptmonitor/isinterruptionrequested/
---
## ThreadInterruptMonitor.IsInterruptionRequested property

Bu uygulama yalnızca zaman maliyetinin (bu izleyicinin başlatıldığı zamandan şimdiye kadar) kullanıcı tarafından belirtilen sınıra göre daha büyük olup olmadığını kontrol eder.

```csharp
public override bool IsInterruptionRequested { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Threading;

    public class ThreadInterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ThreadInterruptMonitor örneği oluşturun
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(terminateWithoutException: false);

            // 2 saniyelik bir sınırla izlemeyi başlatın
            monitor.StartMonitor(2000);

            // Uzun süren bir işlemi simüle edin
            Console.WriteLine("Starting long operation...");
            for (int i = 0; i < 100; i++)
            {
                // Kesintinin istenip istenmediğini kontrol et
                if (monitor.IsInterruptionRequested)
                {
                    Console.WriteLine("Operation was interrupted!");
                    break;
                }

                // İşi simüle edin
                Thread.Sleep(100);
                worksheet.Cells[i, 0].Value = $"Processed row {i}";
                Console.WriteLine($"Processed row {i}");
            }

            // İzlemeyi tamamlayın
            monitor.FinishMonitor();

            // Sonucu kaydet
            workbook.Save("ThreadInterruptionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


