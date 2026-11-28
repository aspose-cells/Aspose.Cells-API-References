---
title: "TxtSaveOptions.AlwaysQuoted"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TxtSaveOptions özelliği. Her alan için her zaman \\\" eklenip eklenmeyeceğini gösterir. True ise tüm değerler tırnak içine alınır. False ise değerler yalnızca gerektiğinde tırnak içine alınır; örneğin değerler özel karakterler içerdiğinde, örneğin   n veya ayırıcı karakter. Varsayılan değer false'tur."
type: docs
url: /tr/net/aspose.cells/txtsaveoptions/alwaysquoted/
---
## TxtSaveOptions.AlwaysQuoted property

Her alan için her zaman '\\"' eklenip eklenmeyeceğini gösterir. True ise tüm değerler tırnak içine alınır; False ise değerler yalnızca gerektiğinde tırnak içine alınır (örneğin, değerler '\\"', '\\n' veya ayırıcı karakter gibi özel karakterler içerdiğinde). Varsayılan değer false'tur.

```csharp
[Obsolete("Use QuoteType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool AlwaysQuoted { get; set; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen QuoteType özelliğini kullanın. Bu özellik, Ağustos 2012'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyAlwaysQuotedDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200.50);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(899.99);

            // AlwaysQuoted özelliği true olarak ayarlanmış TxtSaveOptions oluşturun
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Separator = ',',
                AlwaysQuoted = true,
                QuoteType = TxtValueQuoteType.Always
            };

            // Tüm değerlerin etrafına tırnak işareti ekleyerek kaydedin
            workbook.Save("AlwaysQuoted_True.txt", saveOptions);

            // False olarak değiştirin ve tekrar kaydedin
            saveOptions.AlwaysQuoted = false;
            workbook.Save("AlwaysQuoted_False.txt", saveOptions);

            Console.WriteLine("Files saved with different AlwaysQuoted settings.");
        }
    }
}
```

### Ayrıca Bakınız

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


