---
title: "FormulaSettings.PreservePaddingSpaces"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormulaSettings özelliği. Formül belirteçleri arasında doldurulan boşlukları ve satır sonlarını, formülleri alırken ve ayarlarken koruyup korumayacağını gösterir. Varsayılan değer false'tur."
type: docs
url: /tr/net/aspose.cells/formulasettings/preservepaddingspaces/
---
## FormulaSettings.PreservePaddingSpaces property

Formülleri alırken ve ayarlarken formül tokenları arasında doldurulan boşlukları ve satır sonlarını koruyup korumayacağını gösterir. Varsayılan değer false'tur.

```csharp
public bool PreservePaddingSpaces { get; set; }
```

### Açıklamalar

Genel olarak bu boşluklar ve satır sonları sadece görsel amaçlıdır, bunları korumak ya da korumamak hesaplanan sonuca etki etmez. Performans açısından, özel bir gereklilik yoksa, formülleri işlerken bunları korumamak daha iyidir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyPreservePaddingSpacesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Dolgu boşluklarıyla formül ayarla
            string formulaWithSpaces = "=SUM( IF( A1:A5 > 10, B1:B5, 0 ) )";
            worksheet.Cells["C1"].Formula = formulaWithSpaces;
            
            // Varsayılan davranış (PreservePaddingSpaces true'dır)
            Console.WriteLine("Formula with spaces preserved: " + worksheet.Cells["C1"].Formula);
            
            // Dolgu boşluklarını kaldırmak için ayarı değiştir
            workbook.Settings.FormulaSettings.PreservePaddingSpaces = false;
            worksheet.Cells["C2"].Formula = formulaWithSpaces;
            
            Console.WriteLine("Formula with spaces removed: " + worksheet.Cells["C2"].Formula);
            
            // Çalışma kitabını kaydedin
            workbook.Save("FormulaSpacesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


