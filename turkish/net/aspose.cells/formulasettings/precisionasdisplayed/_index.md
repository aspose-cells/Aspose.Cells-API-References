---
title: "FormulaSettings.PrecisionAsDisplayed"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormulaSettings özelliği. Hesaplanan sonucun hassasiyetinin, formüller hesaplanırken gösterildiği gibi ayarlanıp ayarlanmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells/formulasettings/precisionasdisplayed/
---
## FormulaSettings.PrecisionAsDisplayed property

Formüller hesaplanırken hesaplanan sonucun hassasiyetinin gösterildiği gibi ayarlanıp ayarlanmayacağını gösterir.

```csharp
public bool PrecisionAsDisplayed { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyPrecisionAsDisplayedDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // PrecisionAsDisplayed değerini true olarak ayarlayın
            workbook.Settings.FormulaSettings.PrecisionAsDisplayed = true;
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // A1 hücresi için görüntüleme biçimini 2 ondalık basamak gösterecek şekilde ayarlayın
            cells["A1"].PutValue(1.23456);
            Style style = cells["A1"].GetStyle();
            style.Number = 2; // Format: 0.00
            cells["A1"].SetStyle(style);
            
            // B1 hücresine A1'e referans veren formülü ayarlayın
            cells["B1"].Formula = "=A1";
            
            // PrecisionAsDisplayed etkinleştirilmiş şekilde formülleri hesaplayın
            workbook.CalculateFormula();
            
            // Sonuçları çıktı olarak ver
            Console.WriteLine("A1 Display Value: " + cells["A1"].StringValue); // Shows 1.23
            Console.WriteLine("B1 Calculated Value: " + cells["B1"].Value);   // Should be 1.23 due to PrecisionAsDisplayed
        }
    }
}
```

### Ayrıca Bakınız

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


