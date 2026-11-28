---
title: "InterruptMonitor.IsInterruptionRequested"
second_title: "Aspose.Cells için .NET API Referansı"
description: "InterruptMonitor özelliği. Monitörü kesinti talep ediyor olarak işaretle"
type: docs
url: /tr/net/aspose.cells/interruptmonitor/isinterruptionrequested/
---
## InterruptMonitor.IsInterruptionRequested property

Monitörü kesinti talep ediyor olarak işaretle

```csharp
public override bool IsInterruptionRequested { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class InterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur ve ilk çalışma sayfasına eriş
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir kesinti izleyicisi oluştur ve onu çalışma kitabına ata
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;

            // IsInterruptionRequested'ın başlangıç durumunu göster
            Console.WriteLine("Initial IsInterruptionRequested value: " + monitor.IsInterruptionRequested);

            // Uzun süren bir veri işleme işlemini simüle et
            Console.WriteLine("Starting data processing...");
            for (int rowIdx = 0; rowIdx < 10000; rowIdx++)
            {
                // 500 satır işlendikten sonra kesinti talep et
                if (rowIdx == 500)
                {
                    monitor.Interrupt();
                    Console.WriteLine("Interrupt requested. IsInterruptionRequested: " + monitor.IsInterruptionRequested);
                }

                // Kesinti talebini kontrol et
                if (monitor.IsInterruptionRequested)
                {
                    Console.WriteLine($"Processing interrupted at row {rowIdx}");
                    break;
                }

                // Veri işleme işlemini simüle et
                worksheet.Cells[rowIdx, 0].Value = $"Row {rowIdx} data";
            }

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("InterruptionDemoOutput.xlsx");
            Console.WriteLine("File saved with partial data due to interruption.");
        }
    }
}
```

### Ayrıca Bakınız

* class [InterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


