---
title: "HtmlSaveOptions.CalculateFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. HTML dosyası kaydedilmeden önce formüllerin hesaplanıp hesaplanmayacağını gösterir."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/calculateformula/
---
## HtmlSaveOptions.CalculateFormula property

HTML dosyası kaydedilmeden önce formüllerin hesaplanıp hesaplanmayacağını gösterir.

```csharp
public bool CalculateFormula { get; set; }
```

### Açıklamalar

Varsayılan değer false'tur.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyCalculateFormulaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına veri ve formüller ekle
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");

            // CalculateFormula özelliği true olarak ayarlanmış HtmlSaveOptions oluştur
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                CalculateFormula = true
            };

            // Çalışma kitabını HTML olarak kaydet - formüller hesaplanacak
            workbook.Save("HtmlWithCalculatedFormulas.html", saveOptions);

            Console.WriteLine("HTML file with calculated formulas created successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


