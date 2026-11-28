---
title: "XmlLoadOptions.IgnoreRootAttributes"
second_title: "Aspose.Cells için .NET API Referansı"
description: "XmlLoadOptions özelliği. Kök öğenin özniteliklerinin göz ardı edilip edilmediğini gösterir"
type: docs
url: /tr/net/aspose.cells/xmlloadoptions/ignorerootattributes/
---
## XmlLoadOptions.IgnoreRootAttributes property

Kök öğenin özniteliklerini yoksayıp yoksamama durumunu gösterir.

```csharp
public bool IgnoreRootAttributes { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyIgnoreRootAttributesDemo
    {
        public static void Run()
        {
            // XML yükleme seçeneklerini oluşturun ve IgnoreRootAttributes özelliğini ayarlayın
            XmlLoadOptions options = new XmlLoadOptions();
            options.IgnoreRootAttributes = true;

            // Seçeneklerle XML dosyasını yükleyin
            Workbook workbook = new Workbook("example.xml", options);

            // Yüklenen XML'den verilere erişin
            string cellValue = workbook.Worksheets[0].Cells["AH8"].StringValue;
            Console.WriteLine("Cell AH8 value: " + cellValue);

            // XLSX olarak kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


