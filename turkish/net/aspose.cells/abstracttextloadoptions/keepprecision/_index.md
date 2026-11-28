---
title: "AbstractTextLoadOptions.KeepPrecision"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AbstractTextLoadOptions özelliği. Uzunluğu 15 ise dize değerinin ayrıştırılıp ayrıştırılmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells/abstracttextloadoptions/keepprecision/
---
## AbstractTextLoadOptions.KeepPrecision property

Uzunluğu 15 ise bir dize değerinin ayrılmayacağını belirtir.

```csharp
public bool KeepPrecision { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyKeepPrecisionDemo
    {
        public static void Run()
        {
            // HTML yükleme seçenekleri oluşturun ve KeepPrecision'ı true olarak ayarlayın
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.KeepPrecision = true;

            // Çalışma kitabını seçeneklerle yükleyin
            Workbook workbook = new Workbook("input.html", loadOptions);

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Hassasiyetin korunduğunu gösterin (ör. birçok ondalık basamağa sahip sayısal değerler)
            Cell cell = worksheet.Cells["A1"];
            Console.WriteLine("Value with precision: " + cell.Value);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


