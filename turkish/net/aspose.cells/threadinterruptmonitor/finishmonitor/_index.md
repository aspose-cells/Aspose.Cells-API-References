---
title: "ThreadInterruptMonitor.FinishMonitor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreadInterruptMonitor yöntemi. Bir prosedür için izleyiciyi sonlandırır"
type: docs
url: /tr/net/aspose.cells/threadinterruptmonitor/finishmonitor/
---
## ThreadInterruptMonitor.FinishMonitor method

Bir prosedür için izleyiciyi sonlandırır.

```csharp
public void FinishMonitor()
```

### Açıklamalar

İzlenen prosedürden sonra bu yöntemi çağırmak, izleyici iş parçacığını daha erken serbest bırakabilir, özellikle prosedür için bir kesinti olmadığında (prosedürün zaman maliyeti belirtilen zaman sınırından daha az olduğunda).

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadInterruptMonitorMethodFinishMonitorDemo
    {
        public static void Run()
        {
            // ThreadInterruptMonitor örneği oluşturun
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);

            // LoadOptions oluştur ve InterruptMonitor'ı ayarla
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // 1 saniyelik zaman aşımıyla izlemeyi başlat
            monitor.StartMonitor(1000);

            try
            {
                // Uzun süren bir işlemi simüle edin
                for (int i = 0; i < 5; i++)
                {
                    System.Threading.Thread.Sleep(200);
                    Console.WriteLine($"Processing step {i + 1}");
                }

                // İşlemin izlenmesini sonlandır
                monitor.FinishMonitor();
                Console.WriteLine("Operation completed successfully");
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

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


