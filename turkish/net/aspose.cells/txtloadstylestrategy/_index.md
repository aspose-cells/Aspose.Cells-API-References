---
title: "Enum TxtLoadStyleStrategy"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.TxtLoadStyleStrategy enum. Dize değerini sayıya veya tarih‑zamanına dönüştürürken ayrıştırılan değerler için stilin nasıl uygulanacağını belirtir"
type: docs
url: /tr/net/aspose.cells/txtloadstylestrategy/
---
## TxtLoadStyleStrategy enumeration

Dize değerini sayıya veya tarih‑zamanına dönüştürürken ayrıştırılan değerlere stilin nasıl uygulanacağını belirtir.

```csharp
public enum TxtLoadStyleStrategy
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Ayrıştırılan değer için stil ayarlamaz. |
| BuiltIn | `1` | Ayrıştırılan değer düz sayısal/tarih‑zaman değerleri olduğunda stili yerleşik sayı/tarih‑zaman olarak ayarlayın. |
| ExactFormat | `2` | Ayrıştırılan değer için tam özel biçimi ayarlayarak biçimlendirilmiş değerin orijinal girdiyle aynı olmasını sağlayın. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TxtLoadStyleStrategyDemo
    {
        public static void TxtLoadStyleStrategyExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek bir CSV içeriği tanımlayın
            string csvContent = "Name,Date,Value\nJohn,2023-01-01,100\nDoe,2023-01-02,200";

            // CSV içeriğini geçici bir dosyaya kaydedin
            string tempCsvFilePath = "sample.csv";
            System.IO.File.WriteAllText(tempCsvFilePath, csvContent);

            // TxtLoadOptions oluşturun ve LoadStyleStrategy'yi ayarlayın
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.LoadStyleStrategy = TxtLoadStyleStrategy.ExactFormat;

            // CSV dosyasını çalışma kitabına yükleyin
            workbook = new Workbook(tempCsvFilePath, loadOptions);

            // Çalışma kitabını bir Excel dosyasına kaydet
            workbook.Save("TxtLoadStyleStrategyExample.xlsx");

            // Geçici CSV dosyasını temizleyin
            System.IO.File.Delete(tempCsvFilePath);

            Console.WriteLine("Workbook created and saved successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


