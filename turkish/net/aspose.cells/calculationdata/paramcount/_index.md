---
title: "CalculationData.ParamCount"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CalculationData özelliği. Parametre sayısını alır"
type: docs
url: /tr/net/aspose.cells/calculationdata/paramcount/
---
## CalculationData.ParamCount property

Parametre sayısını alır.

```csharp
public int ParamCount { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyParamCountDemo
    {
        public static void Run()
        {
            try
            {
                // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Parametre olarak kullanılacak bazı hücreleri doldur
                sheet.Cells["A1"].PutValue(10);
                sheet.Cells["A2"].PutValue(20);
                sheet.Cells["A3"].PutValue(30);

                // Üç argümanla bir özel fonksiyonu çağıran bir formül ayarla
                sheet.Cells["B1"].Formula = "=DEMOPARAM(A1, A2, A3)";

                // Özel bir motor kullanmak için hesaplama seçeneklerini yapılandırın
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new ParamCountEngine();

                // Hesaplamayı gerçekleştir
                workbook.CalculateFormula(options);

                // Özel motor, ParamCount değerini hesaplanmış değer olarak döndürür
                Console.WriteLine("ParamCount reported by custom function: " + sheet.Cells["B1"].Value);
                
                // İsteğe bağlı olarak çalışma kitabını kaydet
                workbook.Save("ParamCountDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // ParamCount özelliğini okuma örneği gösteren özel hesaplama motoru
        private class ParamCountEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                // Özel işlevi isimle tanımla
                if (data.FunctionName != null && data.FunctionName.Equals("DEMOPARAM", StringComparison.OrdinalIgnoreCase))
                {
                    // Salt okunur ParamCount özelliğini oku
                    int count = data.ParamCount;

                    // Sayımı işlevin sonucu olarak kullan
                    data.CalculatedValue = count;
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


