---
title: "InterruptMonitor sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.InterruptMonitor sınıfı. Kesintiye ilişkin tüm operatörleri temsil eder"
type: docs
url: /tr/net/aspose.cells/interruptmonitor/
---
## InterruptMonitor class

Kesintiyle ilgili tüm operatörleri temsil eder.

```csharp
public class InterruptMonitor : AbstractInterruptMonitor
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [InterruptMonitor](interruptmonitor/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/interruptmonitor/isinterruptionrequested/) { get; } | Monitörü kesinti talep ediyor olarak işaretle |
| virtual [TerminateWithoutException](../../aspose.cells/abstractinterruptmonitor/terminatewithoutexception/) { get; } | İşlem kesintiye uğradığında, işlemi sessizce sonlandırıp sonlandırmayacağını veya bir Exception fırlatıp fırlatmayacağını belirler. Varsayılan değer false'tur, yani [`IsInterruptionRequested`](../abstractinterruptmonitor/isinterruptionrequested/) true olduğunda, kodu Interrupted olan bir [`CellsException`](../cellsexception/) fırlatılacaktır. ([`AbstractInterruptMonitor`](../abstractinterruptmonitor/) sınıfından kalıtılmıştır.) |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Interrupt](../../aspose.cells/interruptmonitor/interrupt/)() | Mevcut operatörü kesintiye uğrat. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassInterruptMonitorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Örnek veri ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Kesinti izleyicisini oluşturun ve atayın
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;
            
            try
            {
                Console.WriteLine("Starting save operation...");
                
                // İşlemin kesintiye uğratılmasını benzetin
                monitor.Interrupt();
                
                // Kaydetmeye çalış (kesintiye uğramalı)
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

### Ayrıca Bakınız

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


