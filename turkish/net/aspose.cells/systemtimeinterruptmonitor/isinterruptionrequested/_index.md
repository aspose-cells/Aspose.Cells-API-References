---
title: "SystemTimeInterruptMonitor.IsInterruptionRequested"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SystemTimeInterruptMonitor özelliği. Bu uygulama, bu monitörü başlatma zamanından şu ana kadar geçen sürenin, kullanıcı tarafından belirtilen sınırlamadan büyük olup olmadığını sadece kontrol eder"
type: docs
url: /tr/net/aspose.cells/systemtimeinterruptmonitor/isinterruptionrequested/
---
## SystemTimeInterruptMonitor.IsInterruptionRequested property

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

    public class SystemTimeInterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // SystemTimeInterruptMonitor örneği oluştur
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);
            
            // 5 saniyelik zaman sınırlamasıyla izlemeyi başlat
            monitor.StartMonitor(5000);

            // İlk IsInterruptionRequested değerini göster
            Console.WriteLine("Initial IsInterruptionRequested: " + monitor.IsInterruptionRequested);

            // Uzun süren bir işlemi simüle et
            Console.WriteLine("Starting long operation...");
            for (int i = 0; i < 100000; i++)
            {
                worksheet.Cells[i, 0].Value = i;
                
                // Kesintinin istenip istenmediğini kontrol et
                if (monitor.IsInterruptionRequested)
                {
                    Console.WriteLine("Operation interrupted after time limit!");
                    break;
                }
            }

            // Son IsInterruptionRequested değerini göster
            Console.WriteLine("Final IsInterruptionRequested: " + monitor.IsInterruptionRequested);

            // Sonucu kaydet
            workbook.Save("PropertyIsInterruptionRequestedDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


