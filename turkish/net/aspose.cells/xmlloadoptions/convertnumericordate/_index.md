---
title: "XmlLoadOptions.ConvertNumericOrDate"
second_title: "Aspose.Cells için .NET API Referansı"
description: "XmlLoadOptions özelliği. XML dosyasındaki değerin sayısal veya tarih olarak dönüştürülüp dönüştürülmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells/xmlloadoptions/convertnumericordate/
---
## XmlLoadOptions.ConvertNumericOrDate property

XML dosyasındaki değerin sayısal veya tarih formatına dönüştürülüp dönüştürülmediğini gösterir.

```csharp
public bool ConvertNumericOrDate { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyConvertNumericOrDateDemo
    {
        public static void Run()
        {
            // XML yükleme seçenekleri oluşturun
            XmlLoadOptions options = new XmlLoadOptions();
            
            // ConvertNumericOrDate'i true (varsayılan) olarak ayarlayın
            options.ConvertNumericOrDate = true;
            Workbook wb1 = new Workbook("input.xml", options);
            Cell cell1 = wb1.Worksheets[0].Cells["A1"];
            Console.WriteLine("With conversion (true): " + cell1.Value + " is type: " + cell1.Type);
            
            // ConvertNumericOrDate'i false olarak ayarlayın
            options.ConvertNumericOrDate = false;
            Workbook wb2 = new Workbook("input.xml", options);
            Cell cell2 = wb2.Worksheets[0].Cells["A1"];
            Console.WriteLine("Without conversion (false): " + cell2.Value + " is type: " + cell2.Type);
            
            // Sonuçları kaydedin
            wb1.Save("output_with_conversion.xlsx");
            wb2.Save("output_without_conversion.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


