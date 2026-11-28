---
title: "TxtLoadOptions.MaxColumnCount"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TxtLoadOptions özelliği. Bir sayfaya içe aktarılacak maksimum sütun sayısı"
type: docs
url: /tr/net/aspose.cells/txtloadoptions/maxcolumncount/
---
## TxtLoadOptions.MaxColumnCount property

Bir sayfa için içe aktarılacak maksimum sütun sayısı.

```csharp
public int MaxColumnCount { get; set; }
```

### Açıklamalar

Bu sınıra aşan sütunlar, [`ExtendToNextSheet`](../extendtonextsheet/) göre yok sayılacak veya bir sonraki sayfaya genişletilecektir. Bu sayı, başlık sütunlarını ([`HeaderColumnsCount`](../headercolumnscount/)) içerir. İzin verilen en büyük değer, ilgili dosya formatının sütun sınırıdır; örneğin xlsx dosyası için 16384'tür. Bu özellik belirtilmemişse veya belirtilen değer pozitif değilse, en büyük sınır da kullanılacaktır.

### Örnekler

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyMaxColumnCountDemo
    {
        public static void Run()
        {
            // Örnek CSV içeriği oluşturun
            string content = "A,B,C,D,E,F,G,H,I,J,K\n" +
                            "1,2,3,4,5,6,7,8,9,10,11\n" +
                            "a,b,c,d,e,f,g,h,i,j,k";

            // MaxColumnCount 5 olarak ayarlanmış TxtLoadOptions oluştur
            TxtLoadOptions options = new TxtLoadOptions
            {
                MaxColumnCount = 5  // Only load first 5 columns
            };

            // Sınırlı sütunlarla CSV'yi yükle
            using (MemoryStream stream = new MemoryStream(Encoding.UTF8.GetBytes(content)))
            {
                Workbook workbook = new Workbook(stream, options);
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // Yüklenen veriyi çıktıla (yalnızca ilk 5 sütun bulunmalı)
                Console.WriteLine("Data loaded with MaxColumnCount = 5:");
                for (int row = 0; row < cells.MaxDataRow + 1; row++)
                {
                    for (int col = 0; col < cells.MaxDataColumn + 1; col++)
                    {
                        Console.Write(cells[row, col].StringValue + "\t");
                    }
                    Console.WriteLine();
                }

                // Yalnızca 5 sütunun yüklendiğini doğrula
                Console.WriteLine($"\nMax loaded columns: {cells.MaxDataColumn + 1}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


