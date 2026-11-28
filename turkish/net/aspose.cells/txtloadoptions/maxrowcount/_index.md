---
title: "TxtLoadOptions.MaxRowCount"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TxtLoadOptions özelliği. Bir sayfaya içe aktarılacak maksimum satır sayısı"
type: docs
url: /tr/net/aspose.cells/txtloadoptions/maxrowcount/
---
## TxtLoadOptions.MaxRowCount property

Bir sayfa için içe aktarılacak maksimum satır sayısı.

```csharp
public int MaxRowCount { get; set; }
```

### Açıklamalar

Bu sınıra aşan satırlar, [`ExtendToNextSheet`](../extendtonextsheet/) göre yok sayılacak veya bir sonraki sayfaya genişletilecektir. Bu sayı, başlık satırlarını ([`HeaderRowsCount`](../headerrowscount/)) içerir. İzin verilen en büyük değer, ilgili dosya formatının satır sınırıdır; örneğin xlsx dosyası için 1048576'dır. Bu özellik belirtilmemişse veya belirtilen değer pozitif değilse, en büyük sınır da kullanılacaktır.

### Örnekler

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyMaxRowCountDemo
    {
        public static void Run()
        {
            // Örnek CSV içeriği oluşturun
            string content = "Header1,Header2,Header3\n" +
                            "Data1,Data2,Data3\n" +
                            "Data4,Data5,Data6\n" +
                            "Data7,Data8,Data9\n" +
                            "Data10,Data11,Data12\n" +
                            "Data13,Data14,Data15\n" +
                            "Data16,Data17,Data18";

            // MaxRowCount 4 olarak ayarlanmış TxtLoadOptions oluştur
            TxtLoadOptions opts = new TxtLoadOptions
            {
                MaxRowCount = 4,  // Only load first 4 rows (including header)
                HeaderRowsCount = 1  // First row is header
            };

            // CSV'yi çalışma kitabına yükle
            using (MemoryStream ms = new MemoryStream(Encoding.UTF8.GetBytes(content)))
            {
                Workbook wb = new Workbook(ms, opts);

                // Yalnızca 4 satırın yüklendiğini doğrula (1 başlık + 3 veri satırı)
                Worksheet sheet = wb.Worksheets[0];
                Console.WriteLine($"Total rows loaded: {sheet.Cells.MaxDataRow + 1}");
                Console.WriteLine($"Row 1 (Header): {sheet.Cells[0, 0].StringValue}");
                Console.WriteLine($"Row 2 (Data): {sheet.Cells[1, 0].StringValue}");
                Console.WriteLine($"Row 3 (Data): {sheet.Cells[2, 0].StringValue}");
                Console.WriteLine($"Row 4 (Data): {sheet.Cells[3, 0].StringValue}");

                // Bu, yalnızca 4 satır (indeks 0-3) yüklediğimiz için null olacaktır
                if (sheet.Cells[4, 0] == null || string.IsNullOrEmpty(sheet.Cells[4, 0].StringValue))
                {
                    Console.WriteLine("Row 5 was not loaded due to MaxRowCount limitation");
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


