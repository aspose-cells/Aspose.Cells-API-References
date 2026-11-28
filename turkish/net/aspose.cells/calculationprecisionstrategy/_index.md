---
title: "Enum CalculationPrecisionStrategy"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.CalculationPrecisionStrategy enum. Hesaplama hassasiyetini yönetmek için stratejileri listeler. IEEE 754 FloatingPoint Arithmetic'in hassasiyet sorunu nedeniyle bazı basit görünen formüller beklenen sonuç olarak hesaplanmayabilir. Örneğin, 0.450.430.02 formülü, operatörle doğrudan operandları hesaplandığında sonuç sıfır olmaz. Bu tür hassasiyet sorunları için bazı özel stratejiler beklenen sonucu verebilir."
type: docs
url: /tr/net/aspose.cells/calculationprecisionstrategy/
---
## CalculationPrecisionStrategy enumeration

İşlem hassasiyetini ele alma stratejilerini listeler. IEEE 754 Kayan Nokta Aritmetiği'nin hassasiyet sorunu nedeniyle, bazı "görünüşte basit" formüller beklenen sonuç olarak hesaplanmayabilir. Örneğin "=-0.45+0.43+0.02" formülünde, operantlar '+' operatörüyle doğrudan hesaplandığında sonuç sıfır olmaz. Bu tür hassasiyet sorunları için bazı özel stratejiler beklenen sonucu verebilir.

```csharp
public enum CalculationPrecisionStrategy
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Hesaplamada hiçbir strateji uygulanmaz. Hesaplama yaparken yalnızca orijinal double değerini operand olarak kullanın ve sonucu doğrudan döndürün. Performans açısından en verimli ve çoğu durumda uygulanabilir. |
| Round | `1` | Hesaplama sonucunu anlamlı basamaklara göre yuvarlar. |
| Decimal | `2` | Mümkün olduğunda operand olarak decimal kullanır. Performans açısından en verimsiz olanıdır. |

### Örnekler

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class CalculationPrecisionStrategyDemo
    {
        public static void CalculationPrecisionStrategyExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Formula");
            worksheet.Cells["A2"].Formula = "=-0.45+0.43+0.02"; // This should ideally equal 0

            // Hesaplama seçeneklerini ayarlayın
            CalculationOptions calcOptions = new CalculationOptions
            {
                IgnoreError = true,
                Recursive = true,
                PrecisionStrategy = CalculationPrecisionStrategy.Round // Using Round strategy
            };

            // Çalışma sayfasındaki formülleri hesapla
            workbook.CalculateFormula(calcOptions);

            // Formülün sonucunu al
            double result = worksheet.Cells["A2"].DoubleValue;

            // Sonucu çıktı olarak ver
            Console.WriteLine("Calculated Result: " + result);

            // Çalışma kitabını kaydedin
            workbook.Save("CalculationPrecisionStrategyExample.xlsx");
            workbook.Save("CalculationPrecisionStrategyExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


