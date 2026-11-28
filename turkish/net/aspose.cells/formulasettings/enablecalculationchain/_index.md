---
title: "FormulaSettings.EnableCalculationChain"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormulaSettings özelliği. Formüller için hesaplama zincirinin etkinleştirilip etkinleştirilmeyeceğini gösterir. Varsayılan false'tur."
type: docs
url: /tr/net/aspose.cells/formulasettings/enablecalculationchain/
---
## FormulaSettings.EnableCalculationChain property

Formüller için hesaplama zincirinin etkinleştirilip etkinleştirilmeyeceğini gösterir. Varsayılan değer false'tur.

```csharp
public bool EnableCalculationChain { get; set; }
```

### Açıklamalar

Çalışma kitabında çok sayıda formül bulunduğunda ve kullanıcı yalnızca küçük bir kısmını değiştirerek bunları tekrar tekrar hesaplamak istediğinde, performans açısından hesaplama zincirini etkinleştirmek faydalı olabilir. Öte yandan, zincir etkinleştirildiğinde, zincir modelinin korunması ekstra bellek gerektirir ve hücre değerini veya formülleri değiştirme gibi bazı diğer işlemler için biraz daha CPU süresi gerekir. Bu özelliği false'tan true'ya değiştirdikten sonra, hesaplama zinciri çalışma kitabının ilk hesaplaması sırasında analiz edilip oluşturulur, bu yüzden ilk hesaplama süresi zincirsiz normal hesaplamadan daha uzun olabilir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyEnableCalculationChainDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek formüller ekle
            worksheet.Cells["A1"].Formula = "=1+2";
            worksheet.Cells["A2"].Formula = "=A1*3";
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";
            
            // Hesaplama zincirini devre dışı bırak
            workbook.Settings.FormulaSettings.EnableCalculationChain = false;
            
            // Formülleri hesapla
            workbook.CalculateFormula();
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with calculation chain disabled.");
        }
    }
}
```

### Ayrıca Bakınız

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


