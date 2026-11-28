---
title: "Cells.MultiThreadReading"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells özelliği. Hücre veri modelinin MultiThread okumasını destekleyip desteklemeyeceğini alır veya ayarlar. Bu özelliğin varsayılan değeri false'tur"
type: docs
url: /tr/net/aspose.cells/cells/multithreadreading/
---
## Cells.MultiThreadReading property

Hücrelerin veri modelinin Çoklu İş Parçacığı okumasını destekleyip desteklemeyeceğini alır veya ayarlar. Bu özelliğin varsayılan değeri false'tur.

```csharp
public bool MultiThreadReading { get; set; }
```

### Açıklamalar

Bu koleksiyondaki Row/Cell nesnelerini aynı anda birden fazla iş parçacığıyla okumak gerekiyorsa, bu özellik true olarak ayarlanmalıdır, aksi takdirde beklenmeyen sonuçlar ortaya çıkabilir. Multi-Thread okumasını desteklemek, bu koleksiyondan Row/Cell nesnelerine erişim performansını düşürebilir. Lütfen bazı özelliklerin Multi-Thread okumasını desteklemediğini unutmayın, örneğin değer biçimlendirme ([`StringValue`](../../cell/stringvalue/), [`DisplayStringValue`](../../cell/displaystringvalue/), vb.). Bu nedenle, bu özellik true olarak ayarlanmış olsa bile, bu API'ler Multi-Thread okuması için hâlâ beklenmeyen sonuçlar verebilir.

### Örnekler

```csharp
using System;
using System.Threading;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMultiThreadReadingDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Multi-thread okumasını etkinleştir
            cells.MultiThreadReading = true;

            // İlk sütun için stil ayarla
            Style style = wb.CreateStyle();
            style.Custom = "yyyy-mm-dd";
            StyleFlag sf = new StyleFlag();
            sf.All = true;
            cells.Columns[0].ApplyStyle(style, sf);

            // Hücreleri örnek veriyle doldurun
            int rowCount = 1000;
            for (int i = 0; i < rowCount; i++)
            {
                cells[i, 0].PutValue(DateTime.Now.AddDays(i).ToOADate());
            }

            // Hücre değerlerini okumak için iş parçacıkları oluştur
            int threadCount = 5;
            int cellsPerThread = rowCount / threadCount;
            int[] finishedCount = new int[1];
            System.Text.StringBuilder errors = new System.Text.StringBuilder();

            for (int i = 0; i < threadCount; i++)
            {
                int start = i * cellsPerThread;
                int end = (i == threadCount - 1) ? rowCount : start + cellsPerThread;
                
                Thread t = new Thread(() => 
                {
                    try
                    {
                        for (int row = start; row < end; row++)
                        {
                            object value = cells[row, 0].Value;
                            Console.WriteLine($"Thread {Thread.CurrentThread.ManagedThreadId}: Cell[{row},0] = {value}");
                        }
                        Interlocked.Increment(ref finishedCount[0]);
                    }
                    catch (Exception ex)
                    {
                        lock (errors)
                        {
                            errors.AppendLine($"Thread {Thread.CurrentThread.ManagedThreadId} error: {ex.Message}");
                        }
                    }
                });
                t.Start();
            }

            // Tüm iş parçacıklarının tamamlanmasını bekle
            while (finishedCount[0] < threadCount)
            {
                Thread.Sleep(200);
            }

            if (errors.Length > 0)
            {
                Console.WriteLine("Errors occurred:");
                Console.WriteLine(errors.ToString());
            }
            else
            {
                Console.WriteLine("All threads completed successfully");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


