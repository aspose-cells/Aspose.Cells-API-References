---
title: "CalculationOptions.UserSpecifiedRefreshDynamicArrayFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CalculationOptions özelliği. Kullanıcının belirtilen formülleri hesaplamadan önce dinamik dizi formüllerinin yenilenme davranışını açıkça belirleyip belirlemediğini gösterir"
type: docs
url: /tr/net/aspose.cells/calculationoptions/userspecifiedrefreshdynamicarrayformula/
---
## CalculationOptions.UserSpecifiedRefreshDynamicArrayFormula property

Kullanıcının, belirtilen formüller hesaplanmadan önce dinamik dizi formüllerinin yenilenme davranışını açıkça belirleyip belirlemediğini gösterir.

```csharp
public bool UserSpecifiedRefreshDynamicArrayFormula { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationOptionsPropertyUserSpecifiedRefreshDynamicArrayFormulaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Örnek bir çalışma sayfası oluşturun
            Worksheet worksheet = workbook.Worksheets[0];

            // Örneği anlamlı kılmak için bazı veriler ekleyin
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // CalculationOptions örneği oluştur
                CalculationOptions options = new CalculationOptions();

                // UserSpecifiedRefreshDynamicArrayFormula özelliğinin mevcut değerini göster
                Console.WriteLine("UserSpecifiedRefreshDynamicArrayFormula value: " +
                    options.UserSpecifiedRefreshDynamicArrayFormula);

                // Özelliğin davranışı nasıl etkilediğini göster
                Console.WriteLine("UserSpecifiedRefreshDynamicArrayFormula has been demonstrated");

                // Sonucu kaydet
                workbook.Save("UserSpecifiedRefreshDynamicArrayFormulaDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


