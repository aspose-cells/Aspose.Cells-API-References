---
title: "CalculationOptions.IgnoreError"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CalculationOptions özelliği. Formüller hesaplanırken karşılaşılan hataların göz ardı edilip edilmeyeceğini gösterir. Hata, desteklenmeyen işlev, dış bağlantılar vb. olabilir. Varsayılan değer true'dur"
type: docs
url: /tr/net/aspose.cells/calculationoptions/ignoreerror/
---
## CalculationOptions.IgnoreError property

Formüller hesaplanırken karşılaşılan hataların göz ardı edilip edilmediğini gösterir. Hata, desteklenmeyen işlev, harici bağlantılar vb. olabilir. Varsayılan değer true'dur.

```csharp
public bool IgnoreError { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyIgnoreErrorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hata yönetimini göstermek için var olmayan bir adlandırılmış aralık ekleyin
            worksheet.Cells["A1"].Formula = "=NONEXISTENTNAME()";
            
            // IgnoreError = false ile hesaplayın (hata fırlatılacak)
            try
            {
                workbook.CalculateFormula(new CalculationOptions() { IgnoreError = false });
                Console.WriteLine("Calculation completed without ignoring errors");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error occurred (expected): " + ex.Message);
            }

            // IgnoreError = true ile hesaplayın (hata bastırılacak)
            try
            {
                workbook.CalculateFormula(new CalculationOptions() { IgnoreError = true });
                Console.WriteLine("Calculation completed while ignoring errors");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error occurred (unexpected): " + ex.Message);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


