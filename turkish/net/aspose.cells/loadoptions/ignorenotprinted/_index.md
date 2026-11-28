---
title: "LoadOptions.IgnoreNotPrinted"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LoadOptions özelliği. Dosyayı doğrudan yazdırırken yazdırılmayan verileri yoksay"
type: docs
url: /tr/net/aspose.cells/loadoptions/ignorenotprinted/
---
## LoadOptions.IgnoreNotPrinted property

Dosyayı doğrudan yazdırırken yazdırılmayan verileri yok say.

```csharp
public bool IgnoreNotPrinted { get; set; }
```

### Açıklamalar

Yalnızca xlsx dosyası için.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyIgnoreNotPrintedDemo
    {
        public static void Run()
        {
            // HTML yükleme seçenekleri oluşturun ve IgnoreNotPrinted özelliğini ayarlayın
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            loadOptions.IgnoreNotPrinted = true;
            loadOptions.AutoFitColsAndRows = true;

            // Belirtilen seçeneklerle HTML dosyasını yükleyin
            Workbook workbook = new Workbook("example.html", loadOptions);
            Worksheet worksheet = workbook.Worksheets[0];

            // IgnoreNotPrinted etkisini hücre stillerini kontrol ederek gösterin
            Console.WriteLine("B3 Cell Color: " + worksheet.Cells["B3"].GetStyle().ForegroundColor);
            Console.WriteLine("B4 Cell Color: " + worksheet.Cells["B4"].GetStyle().ForegroundColor);
            Console.WriteLine("B5 Cell Color: " + worksheet.Cells["B5"].GetStyle().ForegroundColor);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


