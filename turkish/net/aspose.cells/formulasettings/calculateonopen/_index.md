---
title: "FormulaSettings.CalculateOnOpen"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormulaSettings özelliği. Çalışma kitabı açıldığında uygulamanın tam bir hesaplama yapması gerekip gerekmediğini gösterir"
type: docs
url: /tr/net/aspose.cells/formulasettings/calculateonopen/
---
## FormulaSettings.CalculateOnOpen property

Uygulamanın çalışma kitabı açıldığında tam bir hesaplama yapması gerekip gerekmediğini gösterir.

```csharp
public bool CalculateOnOpen { get; set; }
```

### Açıklamalar

Bu özellik yalnızca ayarları sonuç elektronik tablo dosyasına kaydetmek içindir, böylece diğer uygulamalar (örneğin ms excel) sonuç dosyasını yüklerken buna göre hareket edebilir. Çoğu kullanıcının uygulamaları için performans düşünülerek, bu özelliğin ne değerde ayarlanmış olursa olsun, çalışma kitabındaki hiçbir formül otomatik olarak hesaplanmaz.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculateOnOpenDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1 hücresine B1'e referans veren formülü ayarlayın
            worksheet.Cells["A1"].Formula = "=B1";
            
            // B1 hücresine değeri ayarlayın
            worksheet.Cells["B1"].PutValue(10);
            
            // Açılışta otomatik formül hesaplamayı devre dışı bırakın
            workbook.Settings.FormulaSettings.CalculateOnOpen = false;
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            // Kaydedilen çalışma kitabını yeniden açın
            Workbook reopenedWorkbook = new Workbook("output.xlsx");
            
            // Açılışta formülün hesaplanmadığını doğrulayın
            Console.WriteLine("A1 value (should be 0 before calculation): " + reopenedWorkbook.Worksheets[0].Cells["A1"].IntValue);
            
            // Formülleri manuel olarak hesaplayın
            reopenedWorkbook.CalculateFormula();
            
            // Formülün hesaplandığını doğrulayın
            Console.WriteLine("A1 value (should be 10 after calculation): " + reopenedWorkbook.Worksheets[0].Cells["A1"].IntValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


