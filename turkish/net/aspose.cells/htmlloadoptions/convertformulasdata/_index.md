---
title: "HtmlLoadOptions.ConvertFormulasData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlLoadOptions özelliği. true ise, dize değeri bir karakterle başladığında dizeyi formüle dönüştürür; varsayılan değer false'tur"
type: docs
url: /tr/net/aspose.cells/htmlloadoptions/convertformulasdata/
---
## HtmlLoadOptions.ConvertFormulasData property

true ise, dize değeri '=' karakteriyle başladığında dizeyi formüle dönüştür, varsayılan değer false'tur.

```csharp
[Obsolete("Use HtmlLoadOptions.HasFormula property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ConvertFormulasData { get; set; }
```

### Açıklamalar

NOT: Bu özellik artık kullanılmamaktadır. Bunun yerine lütfen HtmlLoadOptions.HasFormula özelliğini kullanın. Bu özellik, Mart 2023'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyConvertFormulasDataDemo
    {
        public static void Run()
        {
            // HtmlLoadOptions bir örnek oluştur.
            HtmlLoadOptions options = new HtmlLoadOptions();

            // ConvertFormulasData özelliğini true olarak ayarla
            options.ConvertFormulasData = true;

            // Belirtilen seçenekleri kullanarak bir HTML dosyasını Çalışma Kitabına yükleyin
            Workbook workbook = new Workbook("input.html", options);

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Formül dönüşümünü göstermek için bazı hücre değerlerini görüntüleyin
            Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("Cell B1 formula: " + worksheet.Cells["B1"].Formula);

            // Çalışma kitabını bir Excel dosyasına kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


