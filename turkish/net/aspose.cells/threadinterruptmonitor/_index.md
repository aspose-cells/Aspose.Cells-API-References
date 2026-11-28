---
title: "Sınıf ThreadInterruptMonitor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ThreadInterruptMonitor sınıfı. Kullanıcı tarafından belirtilen süre uyuyakaldıktan sonra kesintiyi zorunlu kılmak için başka bir iş parçacığı başlatarak AbstractInterruptMonitor'ın basit bir uygulaması"
type: docs
url: /tr/net/aspose.cells/threadinterruptmonitor/
---
## ThreadInterruptMonitor class

Kullanıcı tarafından belirtilen süre uyuyakaldıktan sonra kesintiyi zorunlu kılmak için başka bir iş parçacığı başlatarak [`AbstractInterruptMonitor`](../abstractinterruptmonitor/) öğesinin basit bir uygulaması.

```csharp
public class ThreadInterruptMonitor : AbstractInterruptMonitor
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [ThreadInterruptMonitor](threadinterruptmonitor/)(bool) | Bir kesinti izleyicisi oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/threadinterruptmonitor/isinterruptionrequested/) { get; } | Bu uygulama yalnızca zaman maliyetinin (bu izleyicinin başlatıldığı zamandan şimdiye kadar) kullanıcı tarafından belirtilen sınıra göre daha büyük olup olmadığını kontrol eder. |
| override [TerminateWithoutException](../../aspose.cells/threadinterruptmonitor/terminatewithoutexception/) { get; } | Bakın [`TerminateWithoutException`](../abstractinterruptmonitor/terminatewithoutexception/). Bu özellik, bu izleyici örneği oluşturulurken kullanıcı tarafından belirtilir. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [FinishMonitor](../../aspose.cells/threadinterruptmonitor/finishmonitor/)() | Bir prosedür için izleyiciyi sonlandırır. |
| [StartMonitor](../../aspose.cells/threadinterruptmonitor/startmonitor/)(int) | İzleyiciyi belirtilen zaman sınırıyla başlatır. Zaman maliyetini hesaplamak için başlangıç zamanı, bu yöntemin çağrıldığı zamandır, bu yüzden izlenmesi gereken prosedür bu çağrının hemen ardından başlatılmalıdır. |

### Açıklamalar

Bir izleyici örneği, her süreci sırasıyla izlediğiniz sürece tekrar tekrar kullanılabilir. Çoklu iş parçacıklarında aynı anda birden fazla prosedürü izlemek için kullanılmamalıdır.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadInterruptMonitorDemo
    {
        public static void ThreadInterruptMonitorExample()
        {
            // terminateWithoutException false olarak ayarlanmış ThreadInterruptMonitor bir örneği oluşturun
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);

            // LoadOptions oluşturun ve InterruptMonitor'ı oluşturulan izleyiciye ayarlayın
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // İzleyiciyi 1000 milisaniye (1 saniye) zaman sınırıyla başlatın
            monitor.StartMonitor(1000);

            try
            {
                // Belirtilen LoadOptions ile bir çalışma kitabı yükleyin
                Workbook wb = new Workbook("Large.xlsx", lopts);

                // Yükleme prosedürü için izleyiciyi sonlandırın
                monitor.FinishMonitor();

                // Yeni bir 1500 milisaniye (1,5 saniye) zaman sınırıyla izleyiciyi tekrar başlatın
                monitor.StartMonitor(1500);

                // Çalışma kitabını kaydedin
                wb.Save("result.xlsx");

                // Kaydetme prosedürü için izleyiciyi sonlandırın
                monitor.FinishMonitor();
            }
            catch (Exception ex)
            {
                Console.WriteLine("An exception occurred: " + ex.Message);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


