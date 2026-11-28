---
title: "FormulaSettings.CalculationMode"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormulaSettings özelliği. MS Excel'de çalışma kitabı hesaplaması için modu alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/formulasettings/calculationmode/
---
## FormulaSettings.CalculationMode property

MS Excel'de çalışma kitabı hesaplama modunu alır veya ayarlar.

```csharp
public CalcModeType CalculationMode { get; set; }
```

### Açıklamalar

Bu özellik yalnızca ayarları ortaya çıkan elektronik tablo dosyasına kaydetmek içindir, böylece diğer uygulamalar (örneğin ms excel) dosyayı yüklerken ve manipüle ederken uygun şekilde davranabilir. Çoğu kullanıcının uygulaması için performans düşünülerek, bu özellik için hangi mod ayarlanmış olursa olsun, çalışma kitabındaki hiçbir formülü otomatik olarak hesaplamıyoruz. Kullanıcı formülleri hesaplaması gerektiğinde, lütfen gereksinime göre farklı nesneler üzerindeki yöntemleri her zaman çağırın: [`CalculateFormula`](../../workbook/calculateformula/), [`CalculateFormula`](../../worksheet/calculateformula/), [`Calculate`](../../cell/calculate/), ... vb.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculationModeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Hesaplama modunu AutomaticExceptTable olarak ayarla
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.AutomaticExceptTable;
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);

            // Hesaplama modunu Manual olarak değiştir
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.Manual;
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);

            // Varsayılan Automatic moduna sıfırla
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.Automatic;
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);
        }
    }
}
```

### Ayrıca Bakınız

* enum [CalcModeType](../../calcmodetype/)
* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


