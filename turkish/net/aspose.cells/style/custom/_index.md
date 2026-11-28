---
title: "Style.Custom"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Bu stil nesnesinin özel sayı biçim dizesini temsil eder. Özel sayı biçimi ayarlanmamışsa, örneğin sayı biçimi yerleşik ise, yerleşik biçim döndürülür."
type: docs
url: /tr/net/aspose.cells/style/custom/
---
## Style.Custom property

Bu stil nesnesinin özel sayı formatı dizesini temsil eder. Özel sayı formatı ayarlanmamışsa (örneğin, sayı formatı yerleşik ise), \"\" döndürülür.

```csharp
public string Custom { get; set; }
```

### Açıklamalar

Döndürülen özel dize kültür bağımsızdır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyCustomDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Özel tarih biçimi oluştur ve uygula
            Style style = workbook.CreateStyle();
            style.Custom = "d-mmm-yy";
            
            cells["A1"].PutValue(new DateTime(2023, 10, 15));
            cells["A1"].SetStyle(style);

            // Biçimlendirilmiş değeri göster
            Console.WriteLine("Formatted value: " + cells["A1"].StringValue);
            
            // Çalışma kitabını kaydedin
            workbook.Save("StylePropertyCustomDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


