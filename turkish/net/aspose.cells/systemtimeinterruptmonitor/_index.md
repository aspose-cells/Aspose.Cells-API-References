---
title: "Sınıf SystemTimeInterruptMonitor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.SystemTimeInterruptMonitor sınıfı. Kullanıcı tarafından belirtilen sınıra göre mevcut sistem zamanını kontrol ederek ve karşılaştırarak AbstractInterruptMonitor'ın basit bir uygulaması"
type: docs
url: /tr/net/aspose.cells/systemtimeinterruptmonitor/
---
## SystemTimeInterruptMonitor class

`[`AbstractInterruptMonitor`](../abstractinterruptmonitor/)` için mevcut sistem zamanını kontrol ederek ve karşılaştırarak basit bir uygulama.

```csharp
public class SystemTimeInterruptMonitor : AbstractInterruptMonitor
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [SystemTimeInterruptMonitor](systemtimeinterruptmonitor/)(bool) | Bir kesinti izleyicisi oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/systemtimeinterruptmonitor/isinterruptionrequested/) { get; } | Bu uygulama yalnızca zaman maliyetinin (bu izleyicinin başlatıldığı zamandan şimdiye kadar) kullanıcı tarafından belirtilen sınıra göre daha büyük olup olmadığını kontrol eder. |
| override [TerminateWithoutException](../../aspose.cells/systemtimeinterruptmonitor/terminatewithoutexception/) { get; } | Bakın [`TerminateWithoutException`](../abstractinterruptmonitor/terminatewithoutexception/). Bu özellik, bu izleyici örneği oluşturulurken kullanıcı tarafından belirtilir. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [StartMonitor](../../aspose.cells/systemtimeinterruptmonitor/startmonitor/)(int) | İzleyiciyi belirtilen zaman sınırıyla başlatır. Zaman maliyetini hesaplamak için başlangıç zamanı, bu yöntemin çağrıldığı zamandır, bu yüzden izlenmesi gereken prosedür bu çağrının hemen ardından başlatılmalıdır. |

### Açıklamalar

Bu uygulama sadece basit senaryolar için basit bir çözümdür. Sistem zamanını sık sık alıp kontrol etmesi gerektiği için performans üzerinde bir miktar olumsuz etkisi olabilir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SystemTimeInterruptMonitorDemo
    {
        public static void SystemTimeInterruptMonitorExample()
        {
            // terminateWithoutException false olarak ayarlanmış SystemTimeInterruptMonitor örneği oluşturun
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);

            // LoadOptions oluşturun ve InterruptMonitor'ı oluşturulan izleyiciye ayarlayın
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // 1000 milisaniye (1 saniye) zaman sınırıyla izlemeyi başlatın
            monitor.StartMonitor(1000);

            try
            {
                // Belirtilen LoadOptions ile bir çalışma kitabı yükleyin
                Workbook wb = new Workbook("Large.xlsx", lopts);

                // Şablon dosyasını yükleme süresi bir saniyeyi aşarsa, kesinti gerekecek ve burada bir istisna fırlatılacak.
                // Aksi takdirde, yeni bir zaman sınırıyla kaydetme prosedürünü izlemeye başlayın.
                monitor.StartMonitor(1500); // time limit is 1.5 seconds

                // Çalışma kitabını kaydedin
                wb.Save("SystemTimeInterruptMonitorExample.xlsx");
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

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


