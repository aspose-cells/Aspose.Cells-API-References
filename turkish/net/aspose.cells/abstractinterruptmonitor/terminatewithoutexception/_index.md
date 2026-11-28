---
title: "AbstractInterruptMonitor.TerminateWithoutException"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AbstractInterruptMonitor özelliği. İşlem kesintiye uğradığında prosedürü sessizce sonlandırıp sonlandırmayacağını veya bir Exception fırlatıp fırlatmayacağını belirler. Varsayılan değer false'tur; yani IsInterruptionRequested true olduğunda kodu Interrupted olan bir CellsException fırlatılacaktır."
type: docs
url: /tr/net/aspose.cells/abstractinterruptmonitor/terminatewithoutexception/
---
## AbstractInterruptMonitor.TerminateWithoutException property

İşlem kesintiye uğradığında, prosedürü sessizce sonlandırıp sonlandırmayacağını veya bir Exception fırlatıp fırlatmayacağını belirler. Varsayılan değer false'tur; yani [`IsInterruptionRequested`](../isinterruptionrequested/) true olduğunda, kodu Interrupted olan bir [`CellsException`](../../cellsexception/) fırlatılacaktır.

```csharp
public virtual bool TerminateWithoutException { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractInterruptMonitorPropertyTerminateWithoutExceptionDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // İşleme yükü oluşturmak için çalışma sayfasını doldur
            for (int row = 0; row < 5000; row++)
            {
                for (int col = 0; col < 50; col++)
                {
                    worksheet.Cells[row, col].Value = "SampleData";
                }
            }

            // SystemTimeInterruptMonitor ile istisna sonlandırmasını göster
            var interruptMonitor1 = new SystemTimeInterruptMonitor(terminateWithoutException: false);
            Console.WriteLine($"Initial TerminateWithoutException: {interruptMonitor1.TerminateWithoutException}");

            workbook.InterruptMonitor = interruptMonitor1;
            interruptMonitor1.StartMonitor(1); // Set 1ms timeout

            try
            {
                workbook.Save("TerminateWithException.xlsx");
                Console.WriteLine("Saved successfully (unexpected with false setting)");
            }
            catch (CellsException ex)
            {
                Console.WriteLine($"Operation terminated with exception: {ex.Message}");
            }

            // SystemTimeInterruptMonitor ile sessiz sonlandırmayı göster
            var interruptMonitor2 = new SystemTimeInterruptMonitor(terminateWithoutException: true);
            Console.WriteLine($"\nNew TerminateWithoutException: {interruptMonitor2.TerminateWithoutException}");

            workbook.InterruptMonitor = interruptMonitor2;
            interruptMonitor2.StartMonitor(1);

            try
            {
                workbook.Save("TerminateSilently.xlsx");
                Console.WriteLine("Saved without exception (expected with true setting)");
            }
            catch (CellsException)
            {
                Console.WriteLine("Exception caught (unexpected with true setting)");
            }

        }
    }

}
```

### Ayrıca Bakınız

* class [AbstractInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


