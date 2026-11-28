---
title: "FormulaSettings.CalculateOnSave"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormulaSettings özelliği. Manuel hesaplama modundayken belgeyi kaydetmeden önce çalışma kitabının yeniden hesaplanıp hesaplanmayacağını gösterir."
type: docs
url: /tr/net/aspose.cells/formulasettings/calculateonsave/
---
## FormulaSettings.CalculateOnSave property

Manuel hesaplama modundayken belgeyi kaydetmeden önce çalışma kitabının yeniden hesaplanıp hesaplanmayacağını gösterir.

```csharp
public bool CalculateOnSave { get; set; }
```

### Açıklamalar

Bu özellik, ayarların ortaya çıkan elektronik tablo dosyasına kaydedilmesi içindir, böylece diğer uygulamalar (örneğin ms excel) dosyayı yüklerken ve üzerinde işlem yaparken uygun şekilde davranabilir. Çoğu kullanıcının uygulamaları için performans açısından, bu özelliğin hangi değere ayarlandığından bağımsız olarak çalışma kitabındaki hiçbir formülü otomatik olarak hesaplamıyoruz.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculateOnSaveDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma sayfasına erişin ve bazı veriler ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // CalculateOnSave'i devre dışı bırak (varsayılan false'tur)
            workbook.Settings.FormulaSettings.CalculateOnSave = false;
            
            // Formülleri hesaplamadan kaydet
            workbook.Save("output_without_calculation.xlsx");

            // CalculateOnSave'i etkinleştir
            workbook.Settings.FormulaSettings.CalculateOnSave = true;
            
            // Formül hesaplamasıyla kaydet
            workbook.Save("output_with_calculation.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


