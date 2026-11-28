---
title: "Enum SignificantDigitsType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.SignificantDigitsType enum. Sayısal değerlerin çıktısı için anlamlı basamak türünü temsil eder"
type: docs
url: /tr/net/aspose.cells/significantdigitstype/
---
## SignificantDigitsType enumeration

Sayısal değerlerin çıktısı için anlamlı basamak türünü temsil eder.

```csharp
public enum SignificantDigitsType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Digits15 | `0` | 15 basamak |
| G17 | `1` | Değeri "G17" ile biçimlendirerek 17 basamak. |
| Rounding17 | `2` | Değeri yuvarlayarak 17 basamak. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassSignificantDigitsTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Demonstrasyon için yeni bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Her SignificantDigitsType enum değerinin kullanımını gösterin
                SignificantDigitsType[] types = {
                    SignificantDigitsType.Digits15,
                    SignificantDigitsType.G17,
                    SignificantDigitsType.Rounding17
                };

                foreach (SignificantDigitsType type in types)
                {
                    // Çalışma kitabı için anlamlı basamak türünü ayarlayın
                    workbook.Settings.SignificantDigitsType = type;

                    // Mevcut ayarı göster
                    Console.WriteLine($"Current SignificantDigitsType: {type} (Value: {(int)type})");

                    // Ayarı göstermek için örnek bir değer ekleyin
                    worksheet.Cells["A1"].PutValue(123.4567890123456789);

                    // Çalışma kitabını mevcut ayarla kaydedin
                    string fileName = $"SignificantDigitsType_{type}.xlsx";
                    workbook.Save(fileName);
                    Console.WriteLine($"Workbook saved with {type} setting as {fileName}");
                }

                Console.WriteLine("All SignificantDigitsType demonstrations completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating SignificantDigitsType: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


