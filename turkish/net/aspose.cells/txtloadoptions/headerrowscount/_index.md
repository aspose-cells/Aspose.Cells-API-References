---
title: "TxtLoadOptions.HeaderRowsCount"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TxtLoadOptions özelliği. Uzatılmış sayfalar için tekrarlanacak başlık satırlarının sayısı"
type: docs
url: /tr/net/aspose.cells/txtloadoptions/headerrowscount/
---
## TxtLoadOptions.HeaderRowsCount property

Genişletilmiş sayfalar için tekrarlanacak başlık satırlarının sayısı.

```csharp
public int HeaderRowsCount { get; set; }
```

### Açıklamalar

Bu özellik tarafından belirtilen başlık satırları, o uzatılmış sayfalar için çoğaltılacaktır. Bu özellik yalnızca [`ExtendToNextSheet`](../extendtonextsheet/) true olduğunda etkili olur.

### Örnekler

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyHeaderRowsCountDemo
    {
        public static void Run()
        {
            // Örnek CSV içeriği oluşturun
            string csvData = "Header1,Header2,Header3\n" +
                            "Value1,Value2,Value3\n" +
                            "Value4,Value5,Value6\n" +
                            "Value7,Value8,Value9";

            // HeaderRowsCount 1 olarak ayarlanmış TxtLoadOptions oluşturun
            TxtLoadOptions options = new TxtLoadOptions
            {
                HeaderRowsCount = 1
            };

            // CSV verisini bir çalışma kitabına yükleyin
            using (MemoryStream stream = new MemoryStream(Encoding.UTF8.GetBytes(csvData)))
            {
                Workbook workbook = new Workbook(stream, options);

                // İlk çalışma sayfasına eriş
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // İlk satırın başlık olarak kabul edildiğini gösterin
                Console.WriteLine("Header Row:");
                for (int col = 0; col < cells.MaxDataColumn + 1; col++)
                {
                    Console.Write(cells[0, col].StringValue + "\t");
                }
                Console.WriteLine("\n");

                // Veri satırlarını göster (başlığı atlayarak)
                Console.WriteLine("Data Rows:");
                for (int row = 1; row < cells.MaxDataRow + 1; row++)
                {
                    for (int col = 0; col < cells.MaxDataColumn + 1; col++)
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


