---
title: "FormulaSettings.CalculationId"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormulaSettings özelliği. Çalışma kitabındaki değerleri hesaplamak için kullanılan hesaplama motorunun sürümünü belirtir."
type: docs
url: /tr/net/aspose.cells/formulasettings/calculationid/
---
## FormulaSettings.CalculationId property

Çalışma kitabındaki değerleri hesaplamak için kullanılan hesaplama motorunun sürümünü belirtir.

```csharp
public string CalculationId { get; set; }
```

### Açıklamalar

Bu özellik, ayarların ortaya çıkan elektronik tablo dosyasına kaydedilmesi içindir, böylece diğer uygulamalar (örneğin ms excel) dosyayı yüklerken ve üzerinde işlem yaparken uygun şekilde davranabilir. ms excel durumunda, bu özelliğin değeri, dosyayı açan uygulamayla ilişkili yeniden hesaplama motoru tanımlayıcısından düşükse, uygulama dosya yüklendikten hemen sonra bu çalışma kitabındaki tüm formüllerin sonuçlarını yeniden hesaplayacaktır. Çoğu kullanıcının uygulamaları için performans açısından, bu özelliğin hangi değere ayarlandığından bağımsız olarak çalışma kitabındaki hiçbir formülü otomatik olarak hesaplamıyoruz.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculationIdDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // CalculationId'ye göre farklı davranan bir formül ayarla
            Cell cell = sheet.Cells["A1"];
            cell.Formula = "=AND(\"a\",true)";
            
            // CalculationId olmadan hesapla (varsayılan davranış)
            wb.CalculateFormula();
            Console.WriteLine("Without CalculationId: " + cell.Value);
            
            // CalculationId'yi ayarla ve yeniden hesapla
            wb.Settings.FormulaSettings.CalculationId = "181029";
            wb.CalculateFormula();
            Console.WriteLine("With CalculationId 181029: " + cell.BoolValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


