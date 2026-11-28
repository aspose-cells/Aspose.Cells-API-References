---
title: "Sınıf AbstractInterruptMonitor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.AbstractInterruptMonitor sınıfı. Tüm zaman alan işlemlerde kesinti isteklerini izleyen bir monitör"
type: docs
url: /tr/net/aspose.cells/abstractinterruptmonitor/
---
## AbstractInterruptMonitor class

Tüm zaman alıcı işlemlerde kesinti isteklerini izlemek için izleme sağlar.

```csharp
public abstract class AbstractInterruptMonitor
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| abstract [IsInterruptionRequested](../../aspose.cells/abstractinterruptmonitor/isinterruptionrequested/) { get; } | Mevcut işlem için kesinti isteği olup olmadığını gösterir. Doğru ise mevcut işlem kesilecektir. Uygulama burada hızlı ve verimli bir kontrol yapmalıdır, aksi takdirde prosedür için başka bir darboğaz haline gelebilir. |
| virtual [TerminateWithoutException](../../aspose.cells/abstractinterruptmonitor/terminatewithoutexception/) { get; } | İşlem kesintiye uğradığında, işlemi sessizce sonlandırıp sonlandırmayacağını veya bir Exception fırlatıp fırlatmayacağını belirler. Varsayılan değer false'tur, yani [`IsInterruptionRequested`](./isinterruptionrequested/) true olduğunda, kodu Interrupted olan bir [`CellsException`](../cellsexception/) fırlatılacaktır. |

### Örnekler

```csharp
using Aspose.Cells;
using System;
using System.Reflection.Metadata.Ecma335;

namespace AsposeCellsExamples
{
    // AbstractInterruptMonitor'ın özel uygulaması
    public class CustomInterruptMonitor : AbstractInterruptMonitor
    {
        //sonuç dosyası doğru
        public override bool IsInterruptionRequested
        {
            get
            {
                Console.WriteLine("Get the return value of whether to interrupt the program===");
                // Kesintinin istenip istenmediğini belirleme mantığı
                return false; // Change this based on your logic
            }
        }

        public override bool TerminateWithoutException
        {
            get => false; // Change this based on your logic
        }

        //// sonuç dosyası çöküyor
        //public override bool IsInterruptionRequested
        //{
        //    get
        //    {
        //        Console.WriteLine("Get the return value of whether to interrupt the program===");
        //        // Kesintinin istenip istenmediğini belirleme mantığı
        //        //return false; // Mantığınıza göre değiştirin
        //        return true;
        //    }
        //}

        //public override bool TerminateWithoutException
        //{
        //    get => true; // Mantığınıza göre değiştirin
        //}
    }

    public class InterruptMonitorDemo
    {
        public static void RunDemo()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].Formula = "=A1+A2";

            // CustomInterruptMonitor'ın bir örneğini oluştur
            CustomInterruptMonitor monitor = new CustomInterruptMonitor();

            // özel kesinti izleyicisiyle yükleme seçeneklerini ayarla
            LoadOptions loadOptions = new LoadOptions
            {
                InterruptMonitor = monitor
            };

            // Belirtilen seçeneklerle çalışma kitabını yükle
            workbook = new Workbook("Sample.xlsx", loadOptions);

            // Hesaplamaları gerçekleştir
            workbook.CalculateFormula();

            // Çalışma kitabını kaydedin
            workbook.Save("InterruptMonitorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


