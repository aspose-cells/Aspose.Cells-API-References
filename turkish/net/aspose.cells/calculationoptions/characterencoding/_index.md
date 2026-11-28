---
title: "CalculationOptions.CharacterEncoding"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CalculationOptions özelliği. Formüller hesaplanırken karakterlerin kodlanması/çözülmesi için kullanılan kodlamayı belirtir. CHAR CODE gibi işlevler için hesaplanan sonuç, bölge ayarları ve ortamın varsayılan karakter kümesine bağlıdır. Bu özellik sayesinde kullanıcı, bu işlevler için beklenen sonucu elde etmek üzere uygun kodlamayı belirtebilir."
type: docs
url: /tr/net/aspose.cells/calculationoptions/characterencoding/
---
## CalculationOptions.CharacterEncoding property

Formüller hesaplanırken karakterlerin kodlanması/kod çözülmesi için kullanılan kodlamayı belirtir. CHAR, CODE gibi işlevler için hesaplanan sonuç bölge ayarları ve ortamın varsayılan karakter kümesine bağlıdır. Bu özellik sayesinde kullanıcı, bu işlevler için beklenen sonucu elde etmek üzere uygun kodlamayı belirtebilir.

```csharp
public Encoding CharacterEncoding { get; set; }
```

### Örnekler

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyCharacterEncodingDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            wb.Settings.Region = CountryCode.Japan;
            
            CalculationOptions copts = new CalculationOptions();
            copts.CharacterEncoding = Encoding.GetEncoding("iso-2022-jp");
            
            string formula = "=TRIM(1)";
            string result = (string)sheet.CalculateFormula(formula, copts);
            
            Console.WriteLine("Calculation result: " + result);
        }
    }
}
```

### Ayrıca Bakınız

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


