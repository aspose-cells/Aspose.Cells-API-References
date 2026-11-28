---
title: "TxtLoadOptions.HeaderColumnsCount"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TxtLoadOptions özelliği. Genişletilmiş sayfalar için tekrarlanacak başlık sütunlarının sayısı"
type: docs
url: /tr/net/aspose.cells/txtloadoptions/headercolumnscount/
---
## TxtLoadOptions.HeaderColumnsCount property

Genişletilmiş sayfalar için tekrarlanacak başlık sütunlarının sayısı.

```csharp
public int HeaderColumnsCount { get; set; }
```

### Açıklamalar

Bu özellik tarafından belirtilen başlık sütunları, genişletilmiş sayfalar için çoğaltılacaktır. Bu özellik yalnızca [`ExtendToNextSheet`](../extendtonextsheet/) true olduğunda etkili olur.

### Örnekler

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyHeaderColumnsCountDemo
    {
        public static void Run()
        {
            // Örnek CSV içeriği oluşturun
            string csvData = "Header1,Header2,Header3,Data1,Data2,Data3\n" +
                            "H1,H2,H3,D1,D2,D3\n" +
                            "A,B,C,D,E,F\n" +
                            "G,H,I,J,K,L";

            // HeaderColumnsCount 3 olarak ayarlanmış TxtLoadOptions oluştur
            TxtLoadOptions options = new TxtLoadOptions
            {
                HeaderColumnsCount = 3, // First 3 columns will be treated as headers
                Encoding = Encoding.UTF8
            };

            // CSV verisini bir çalışma kitabına yükleyin
            using (MemoryStream stream = new MemoryStream(Encoding.UTF8.GetBytes(csvData)))
            {
                Workbook workbook = new Workbook(stream, options);
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // Başlık sütunlarını göster (ilk 3 sütun)
                Console.WriteLine("Header Columns:");
                for (int row = 0; row < 2; row++)
                {
                    for (int col = 0; col < options.HeaderColumnsCount; col++)
                    {
                        Console.Write(cells[row, col].StringValue + "\t");
                    }
                    Console.WriteLine();
                }

                // Veri sütunlarını göster (kalan sütunlar)
                Console.WriteLine("\nData Columns:");
                for (int row = 0; row < cells.MaxDataRow + 1; row++)
                {
                    for (int col = options.HeaderColumnsCount; col < cells.MaxDataColumn + 1; col++)
                    {
                        Console.Write(cells[row, col].StringValue + "\t");
                    }
                    Console.WriteLine();
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


