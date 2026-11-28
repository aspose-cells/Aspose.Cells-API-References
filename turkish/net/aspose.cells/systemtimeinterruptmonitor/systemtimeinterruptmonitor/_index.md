---
title: "SystemTimeInterruptMonitor.SystemTimeInterruptMonitor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SystemTimeInterruptMonitor yapıcı. Bir kesinti izleyici oluşturur"
type: docs
url: /tr/net/aspose.cells/systemtimeinterruptmonitor/systemtimeinterruptmonitor/
---
## SystemTimeInterruptMonitor constructor

Bir kesinti izleyicisi oluşturur.

```csharp
public SystemTimeInterruptMonitor(bool terminateWithoutException)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| terminateWithoutException | Boolean | [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/) |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SystemTimeInterruptMonitorMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // terminateWithoutException false olarak ayarlanmış bir örnek oluştur
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);

            // İzleyici ile yükleme seçeneklerini ayarla
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // 1 saniyelik zaman sınırıyla izlemeyi başlat
            monitor.StartMonitor(1000);

            try
            {
                // Çalışma kitabını yüklemeyi dene
                Workbook wb = new Workbook("sample.xlsx", lopts);

                // Kaydetme işlemi için monitörü 1,5 saniyelik sınırlama ile sıfırla
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

### Ayrıca Bakınız

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


