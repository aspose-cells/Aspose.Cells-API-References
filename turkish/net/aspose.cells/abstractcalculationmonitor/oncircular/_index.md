---
title: "AbstractCalculationMonitor.OnCircular"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AbstractCalculationMonitor yöntemi. Döngüsel referanslı formüller hesaplanırken iş mantığını gerçekleştirmek için bu yöntemi uygulayın"
type: docs
url: /tr/net/aspose.cells/abstractcalculationmonitor/oncircular/
---
## AbstractCalculationMonitor.OnCircular method

Dairesel referanslarla formüller hesaplanırken bu yöntemi uygulayın.

```csharp
public virtual bool OnCircular(IEnumerator circularCellsData)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| circularCellsData | IEnumerator | Döngüsel referanslara bağımlı hücreleri temsil eden [`CalculationCell`](../../calculationcell/) öğeleriyle IEnumerator. |

### Dönüş Değeri

Bu çağrıdan sonra formül motorunun bu hücreleri döngü içinde hesaplaması gerekip gerekmediği. Doğru ise formül motorunun onlar için hesaplamaya devam etmesine izin verir. Yanlış ise formül motorunun bu hücreleri sadece Calculated olarak işaretlemesine izin verir.

### Açıklamalar

Uygulamada kullanıcı, bu hücrelerin bir kısmı/ tamamı için beklenen değeri hesaplanmış sonuç olarak ayarlayabilir, böylece formül motoru onları yinelemeli olarak hesaplamaz.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class AbstractCalculationMonitorMethodOnCircularDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Döngüsel referans senaryosu oluştur
            worksheet.Cells["A1"].Formula = "=B1";
            worksheet.Cells["B1"].Formula = "=A1";

            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = new CircularReferenceMonitor();

            try
            {
                workbook.CalculateFormula(options);
                Console.WriteLine("Calculation completed. Check console for circular reference handling.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Calculation error: {ex.Message}");
            }

            workbook.Save("OnCircularDemo.xlsx");
        }

        private class CircularReferenceMonitor : AbstractCalculationMonitor
        {
            public override bool OnCircular(IEnumerator circularCellsData)
            {
                Console.WriteLine("Circular reference detected!");
                while (circularCellsData.MoveNext())
                {
                    Console.WriteLine($"Circular cell: {circularCellsData.Current}");
                }
                return true; // Continue calculation
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


