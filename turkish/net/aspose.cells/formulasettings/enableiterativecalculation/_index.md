---
title: "FormulaSettings.EnableIterativeCalculation"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormulaSettings özelliği. Döngüsel referansları çözmek için yinelemeli hesaplamayı etkinleştirip etkinleştirmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells/formulasettings/enableiterativecalculation/
---
## FormulaSettings.EnableIterativeCalculation property

Döngüsel referansları çözmek için yinelemeli hesaplamanın etkinleştirilip etkinleştirilmeyeceğini gösterir.

```csharp
public bool EnableIterativeCalculation { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyEnableIterativeCalculationDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Gösterim için döngüsel referans kurun
            worksheet.Cells["A1"].Formula = "=B1+1";
            worksheet.Cells["B1"].Formula = "=A1+1";
            
            // Azami yineleme sayısıyla yinelemeli hesaplamayı etkinleştirin
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 100;
            workbook.Settings.FormulaSettings.MaxChange = 0.001;
            
            // Formülleri hesapla
            workbook.CalculateFormula();
            
            // Sonuçları çıktı olarak ver
            Console.WriteLine("A1 value after calculation: " + worksheet.Cells["A1"].DoubleValue);
            Console.WriteLine("B1 value after calculation: " + worksheet.Cells["B1"].DoubleValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


