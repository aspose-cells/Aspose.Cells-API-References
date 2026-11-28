---
title: "Enum TxtValueQuoteType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.TxtValueQuoteType enum. Metin biçimindeki dosyalardaki değerler için tırnak işareti kullanım türünü belirtir"
type: docs
url: /tr/net/aspose.cells/txtvaluequotetype/
---
## TxtValueQuoteType enumeration

Metin biçimindeki dosyalardaki değerler için tırnak işareti kullanım türünü belirtir.

```csharp
public enum TxtValueQuoteType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Normal | `0` | Tırnak işareti, ayırıcı karakter gibi özel karakterler içeren tüm değerler tırnak içine alınır. Metin dosyası dışa aktarırken ms excel davranışıyla aynıdır. |
| Always | `1` | Tüm değerler her zaman tırnak içine alınır. |
| Minimum | `2` | Değerler yalnızca gerektiğinde tırnak içine alınır. Örneğin, bir değer tırnak işareti içeriyorsa ancak tırnak işareti değerin başında değilse, bu değer tırnak içine alınmaz. |
| Never | `3` | Tüm değerler tırnak içine alınmaz. Bu türle dışa aktarılan metin dosyası, gerekli tırnak işaretleri eksik olduğu için doğru şekilde geri okunamayabilir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TxtValueQuoteTypeDemo
    {
        public static void TxtValueQuoteTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı veriler ekle
            worksheet.Cells[0, 0].Value = "Name";
            worksheet.Cells[0, 1].Value = "Age";
            worksheet.Cells[1, 0].Value = "John Doe";
            worksheet.Cells[1, 1].Value = 30;
            worksheet.Cells[2, 0].Value = "Jane Smith";
            worksheet.Cells[2, 1].Value = 25;

            // TxtSaveOptions oluştur ve QuoteType'ı ayarla
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.QuoteType = TxtValueQuoteType.Always;

            // Çalışma kitabını belirtilen tırnak türüyle metin dosyası olarak kaydet
            workbook.Save("TxtValueQuoteTypeExample.txt", saveOptions);

            Console.WriteLine("Workbook saved with TxtValueQuoteType.Always");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


