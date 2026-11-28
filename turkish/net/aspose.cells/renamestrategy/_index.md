---
title: "Enum RenameStrategy"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.RenameStrategy enum. Sütunların yinelenen adları için strateji seçeneği"
type: docs
url: /tr/net/aspose.cells/renamestrategy/
---
## RenameStrategy enumeration

Sütunların yinelenen adları için strateji seçeneği.

```csharp
public enum RenameStrategy
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Exception | `0` | İstisna fırlatır. |
| Digit | `1` | Rakamla adlandırılmıştır. Yinelenen adlar ...1, ...2, vb. şeklinde olur. |
| Letter | `2` | Harfle adlandırılmıştır. Yinelenen adlar ...A, ...B, vb. şeklinde olur. |

### Açıklamalar

Başlıklarla veri işlenirken, bazı senaryolar tüm sütunlar için başlıkların tekrarsız olmasını gerektirir. Örneğin, verileri bir DataTable’a dışa aktarırken başlığın DataTable’ın sütun adı olarak alınması gerekiyorsa, başlığın yinelenen değerleri geçersizdir. Bu tür durumlarda kullanıcı, bu stratejiyi belirterek nasıl ele alınacağını seçebilir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RenameStrategyDemo
    {
        public static void RenameStrategyExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı örnek veriler ekleyin
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("John");

            // ExportTableOptions oluşturun ve RenameStrategy'yi ayarlayın
            ExportTableOptions options = new ExportTableOptions
            {
                RenameStrategy = RenameStrategy.Digit // Use the Digit strategy for duplicate names
            };

            // Çalışma sayfası verilerini bir DataTable’a dışa aktar
            System.Data.DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 4, 1, options);

            // DataTable içeriğini göster
            foreach (System.Data.DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item + "\t");
                }
                Console.WriteLine();
            }

            // Çalışma kitabını kaydedin
            workbook.Save("RenameStrategyExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


