---
title: "FormulaSettings.ForceFullCalculation"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormulaSettings özelliği. Bir hesaplama tetiklendiğinde tüm formüllerin her seferinde hesaplanıp hesaplanmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/formulasettings/forcefullcalculation/
---
## FormulaSettings.ForceFullCalculation property

Bir hesaplama tetiklendiğinde tüm formüllerin her seferinde hesaplanıp hesaplanmayacağını gösterir.

```csharp
public bool ForceFullCalculation { get; set; }
```

### Açıklamalar

Bu özellik, ayarların ortaya çıkan elektronik tablo dosyasına kaydedilmesi içindir, böylece diğer uygulamalar (örneğin ms excel) dosyayı yüklerken ve üzerinde işlem yaparken uygun şekilde davranabilir. Çoğu kullanıcının uygulamaları için performans açısından, bu özelliğin hangi değere ayarlandığından bağımsız olarak çalışma kitabındaki hiçbir formülü otomatik olarak hesaplamıyoruz.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyForceFullCalculationDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Formül ayarlarına erişin
            FormulaSettings formulaSettings = workbook.Settings.FormulaSettings;

            // ForceFullCalculation özelliğini gösterin
            formulaSettings.ForceFullCalculation = true;
            Console.WriteLine($"ForceFullCalculation is set to: {formulaSettings.ForceFullCalculation}");

            // Örnek veri ve formül ekle
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // ForceFullCalculation ayarıyla formülleri hesaplayın
            workbook.CalculateFormula();

            // Sonucu çıktı olarak ver
            Console.WriteLine($"Calculation result: {worksheet.Cells["A3"].Value}");

            // Çalışma kitabını kaydedin
            workbook.Save("ForceFullCalculationDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


