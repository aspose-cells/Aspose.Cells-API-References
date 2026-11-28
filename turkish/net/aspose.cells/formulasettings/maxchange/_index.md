---
title: "FormulaSettings.MaxChange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormulaSettings özelliği. Döngüsel referansı çözmek için maksimum değişiklik"
type: docs
url: /tr/net/aspose.cells/formulasettings/maxchange/
---
## FormulaSettings.MaxChange property

Döngüsel bir referansı çözmek için azami değişim.

```csharp
public double MaxChange { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyMaxChangeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Yinelemeli hesaplama ayarlarını kur
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 100;
            workbook.Settings.FormulaSettings.MaxChange = 0.001; // Set maximum change threshold
            
            // Demonstrasyon için döngüsel referans oluştur
            worksheet.Cells["A1"].Formula = "=B1+1";
            worksheet.Cells["B1"].Formula = "=A1+1";
            
            // Belirtilen MaxChange ayarıyla formülleri hesapla
            workbook.CalculateFormula();
            
            // Sonuçları çıktı olarak ver
            Console.WriteLine("A1 value: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("B1 value: " + worksheet.Cells["B1"].Value);
            Console.WriteLine("MaxChange used: " + workbook.Settings.FormulaSettings.MaxChange);
        }
    }
}
```

### Ayrıca Bakınız

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


