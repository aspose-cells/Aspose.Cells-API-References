---
title: "CellsHelper.SignificantDigitsType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsHelper özelliği. Sayısal değerleri çıktıya alırken kullanılan varsayılan anlamlı basamak tipini alır ve ayarlar. Varsayılan değer G17"
type: docs
url: /tr/net/aspose.cells/cellshelper/significantdigitstype/
---
## CellsHelper.SignificantDigitsType property

Sayısal değerleri çıkartmak için varsayılan önemli basamak tipini alır ve ayarlar. Varsayılan değer G17'dir.

```csharp
public static SignificantDigitsType SignificantDigitsType { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperPropertySignificantDigitsTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Geçerli SignificantDigitsType değerini göster
                Console.WriteLine("Current SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // Yeni bir SignificantDigitsType değeri ayarla
                CellsHelper.SignificantDigitsType = SignificantDigitsType.G17;
                Console.WriteLine("Updated SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // Etkiyi göstermek için bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Anlamlı basamaklardan etkilenecek bir sayısal değer ekle
                worksheet.Cells["A1"].PutValue(1.2345678912345678);
                worksheet.Cells["A2"].PutValue(1.2345678912345678);
                worksheet.Cells["A3"].Formula = "=A1+A2";

                // Geçerli anlamlı basamak tipini kullanarak formülleri hesapla
                workbook.CalculateFormula();

                // Sonucu göster
                Console.WriteLine("Calculation result: " + worksheet.Cells["A3"].Value);

                // Başka bir anlamlı basamak tipine değiştir
                CellsHelper.SignificantDigitsType = SignificantDigitsType.Rounding17;
                Console.WriteLine("Changed SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // Yeni anlamlı basamak tipiyle yeniden hesapla
                workbook.CalculateFormula();
                Console.WriteLine("Recalculated result: " + worksheet.Cells["A3"].Value);

                // Çalışma kitabını kaydedin
                workbook.Save("SignificantDigitsTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [SignificantDigitsType](../../significantdigitstype/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


