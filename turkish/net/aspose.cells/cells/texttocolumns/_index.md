---
title: "Cells.TextToColumns"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Belirtilen sütundaki içeriği birden fazla sütuna böler"
type: docs
url: /tr/net/aspose.cells/cells/texttocolumns/
---
## Cells.TextToColumns method

Belirtilen sütundaki içeriği birden çok sütuna böler..

```csharp
public int TextToColumns(int row, int column, int totalRows, TxtLoadOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Satır indeksi. |
| sütun | Int32 | Sütun indeksi. |
| totalRows | Int32 | Satır sayısı. |
| seçenekler | TxtLoadOptions | Bölme seçenekleri. |

### Dönüş Değeri

Bölünmüş değerlerin toplam sütun sayısı.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodTextToColumnsWithInt32Int32Int32TxtLoadOptionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Virgülle ayrılmış değerlerle örnek veri ayarla
            sheet.Cells["A1"].PutValue("John,Doe,30");
            sheet.Cells["A2"].PutValue("Jane,Smith,28");

            // Virgülü ayırıcı olarak kullanarak metin yükleme seçenekleri oluştur
            TxtLoadOptions options = new TxtLoadOptions();
            options.Separator = ',';

            // Metni A1 hücresinden başlayarak 3 sütun genişliğinde sütunlara böl
            sheet.Cells.TextToColumns(0, 0, 3, options);

            // Sonuçları doğrulayın
            Console.WriteLine("B1: " + sheet.Cells["B1"].StringValue); // Should output "Doe"
            Console.WriteLine("C2: " + sheet.Cells["C2"].StringValue); // Should output "28"

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


