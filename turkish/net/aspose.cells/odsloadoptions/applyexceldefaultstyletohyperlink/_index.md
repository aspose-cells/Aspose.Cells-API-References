---
title: "OdsLoadOptions.ApplyExcelDefaultStyleToHyperlink"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OdsLoadOptions özelliği. Excel'in varsayılan stilinin bağlantıya uygulanıp uygulanmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/odsloadoptions/applyexceldefaultstyletohyperlink/
---
## OdsLoadOptions.ApplyExcelDefaultStyleToHyperlink property

Excel'in varsayılan stilinin köprüye uygulanıp uygulanmayacağını gösterir.

```csharp
public bool ApplyExcelDefaultStyleToHyperlink { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OdsLoadOptionsPropertyApplyExcelDefaultStyleToHyperlinkDemo
    {
        public static void Run()
        {
            // OdsLoadOptions sınıfının bir örneğini oluşturun
            OdsLoadOptions loadOptions = new OdsLoadOptions();

            // ApplyExcelDefaultStyleToHyperlink özelliğini ayarla
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;

            // Belirtilen seçeneklerle bir ODS dosyası yükleyin
            Workbook workbook = new Workbook("sample.ods", loadOptions);

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Stil uygulamasını göstermek için bir bağlantı ekle
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            // Çalışma kitabını yeni bir dosyaya kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


