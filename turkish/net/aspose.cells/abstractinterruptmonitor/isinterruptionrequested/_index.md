---
title: "AbstractInterruptMonitor.IsInterruptionRequested"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AbstractInterruptMonitor özelliği. Mevcut işlem için kesintinin istenip istenmediğini gösterir. True ise mevcut işlem kesilecektir. Uygulama burada hızlı ve verimli bir kontrol yapmalıdır, aksi takdirde prosedür için başka bir darboğaz haline gelebilir"
type: docs
url: /tr/net/aspose.cells/abstractinterruptmonitor/isinterruptionrequested/
---
## AbstractInterruptMonitor.IsInterruptionRequested property

Mevcut işlem için kesinti isteği olup olmadığını gösterir. Doğru ise mevcut işlem kesilecektir. Uygulama burada hızlı ve verimli bir kontrol yapmalıdır, aksi takdirde prosedür için başka bir darboğaz haline gelebilir.

```csharp
public abstract bool IsInterruptionRequested { get; }
```

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kesinti izleyicisi oluşturun ve çalışma kitabına atayın
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;

            // İlk değeri göster
            Console.WriteLine("Initial IsInterruptionRequested: " + monitor.IsInterruptionRequested);

            // Kesinti görevini başlat
            Task.Run(() =>
            {
                Thread.Sleep(1000); // Wait 1 seconds
                Console.WriteLine("\nTriggering interruption...");
                monitor.Interrupt();
            });

            // Uzun süren işlem simülasyonu
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
                    
                    // İşleme süresini simüle et
                    if (i % 1000 == 0) 
                        Console.Write(".");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine("\nError: " + ex.Message);
            }

            // Sonucu kaydedin
            workbook.Save("InterruptionDemoOutput.xlsx");

            Console.WriteLine("\nWorkbook saved with partial data.");
        }
    }
}
```

### Ayrıca Bakınız

* class [AbstractInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


