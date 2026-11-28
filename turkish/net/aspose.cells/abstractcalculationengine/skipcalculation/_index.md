---
title: "AbstractCalculationEngine.SkipCalculation"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AbstractCalculationEngine yöntemi. Şu anda değerlendirilmekte olan işlevi referans alan tüm formülün hesaplamasını atlar"
type: docs
url: /tr/net/aspose.cells/abstractcalculationengine/skipcalculation/
---
## AbstractCalculationEngine.SkipCalculation method

Şu anda değerlendirilmekte olan fonksiyona başvuran tüm formülün hesaplamasını atlar.

```csharp
public void SkipCalculation()
```

### Açıklamalar

Bu yöntem, tüm formülün hesaplamasını atlamak için [`Calculate`](../calculate/) uygulamasında çağrılabilir ve formülün orijinal değeri değişmeden korunur.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationEngineMethodSkipCalculationDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bağlam için bazı veriler ekle
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Formula = "=SKIPFUNC(A1,A2)";

            // Özel bir hesaplama motoru oluştur
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomSkipEngine();

            try
            {
                // Özel motorumuzu tetikleyecek şekilde çalışma kitabını hesapla
                workbook.CalculateFormula(options);

                // Sonucu göster (atlanmalı)
                Console.WriteLine("Calculation result: " + worksheet.Cells["A3"].StringValue);

                // Çalışma kitabını kaydedin
                workbook.Save("SkipCalculationDemo.xlsx");
                Console.WriteLine("SkipCalculation method demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating SkipCalculation: {ex.Message}");
            }
        }
    }

    public class CustomSkipEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName.ToUpper() == "SKIPFUNC")
            {
                // Bu formülün hesaplamasını atla
                SkipCalculation();
                data.CalculatedValue = "#SKIPPED!";
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


