---
title: "CalculationOptions.RefreshDynamicArrayFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CalculationOptions özelliği. Dinamik dizi formüllerinin formüller hesaplanmadan önce yenilenip yenilenmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells/calculationoptions/refreshdynamicarrayformula/
---
## CalculationOptions.RefreshDynamicArrayFormula property

Dinamik dizi formüllerinin formüller hesaplanmadan önce yenilenip yenilenmeyeceğini gösterir.

```csharp
public bool RefreshDynamicArrayFormula { get; set; }
```

### Açıklamalar

Eğer bu özellik açıkça belirtilmişse, belirtilen değer dinamik dizi formüllerinin yenilenip yenilenmeyeceğini belirlemek için kullanılacaktır. Aksi takdirde ([`UserSpecifiedRefreshDynamicArrayFormula`](../userspecifiedrefreshdynamicarrayformula/) yanlış), varsayılan değeri, hesaplanması gereken formül türüne bağlıdır: Çalışma kitabı için formülleri hesaplamak gibi, [`CalculateFormula`](../../workbook/calculateformula/) durumunda, bu özellik true olarak alınır. Diğer durumlarda, örneğin [`Calculate`](../../cell/calculate/) veya [`CalculateFormula`](../../worksheet/calculateformula/) gibi, bu özellik false olarak alınır.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationOptionsPropertyRefreshDynamicArrayFormulaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // İşlevselliği göstermek için bir dinamik dizi formülü ekle
            worksheet.Cells["A1"].Value = 1;
            worksheet.Cells["A2"].Value = 2;
            worksheet.Cells["A3"].Value = 3;
            worksheet.Cells["B1"].Formula = "=A1:A3"; // Dynamic array formula

            // CalculationOptions örneği oluştur
            CalculationOptions options = new CalculationOptions();

            try
            {
                // RefreshDynamicArrayFormula varsayılan değerini göster
                Console.WriteLine("Default RefreshDynamicArrayFormula value: " + options.RefreshDynamicArrayFormula);

                // Dinamik dizi formüllerini yenilemek için özelliği true olarak ayarla
                options.RefreshDynamicArrayFormula = true;
                Console.WriteLine("After setting to true: " + options.RefreshDynamicArrayFormula);

                // Belirtilen seçeneklerle formülleri hesapla
                workbook.CalculateFormula(options);

                // Hesaplanan sonucu gösterin
                Console.WriteLine("Dynamic array formula result: " + worksheet.Cells["B1"].Value);

                // Çalışma kitabını kaydedin
                workbook.Save("RefreshDynamicArrayFormulaDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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


