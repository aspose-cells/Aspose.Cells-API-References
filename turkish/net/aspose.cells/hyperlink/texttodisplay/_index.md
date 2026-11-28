---
title: "Hyperlink.TextToDisplay"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Hyperlink özelliği. Belirtilen köprü için görüntülenecek metni temsil eder. Varsayılan değer köprünün adresidir"
type: docs
url: /tr/net/aspose.cells/hyperlink/texttodisplay/
---
## Hyperlink.TextToDisplay property

Belirtilen köprü için görüntülenecek metni temsil eder. Varsayılan değer köprünün adresidir.

```csharp
public string TextToDisplay { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyTextToDisplayDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // TextToDisplay özelliğiyle köprüler ekleyin
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;
            
            // Özel görüntüleme metniyle ilk köprüyü ekleyin
            int index1 = hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            hyperlinks[index1].TextToDisplay = "Visit Aspose Website";
            
            // Özel görüntüleme metniyle ikinci bağlantıyı ekle
            int index2 = hyperlinks.Add("A2", 1, 1, "https://docs.aspose.com");
            hyperlinks[index2].TextToDisplay = "Aspose Documentation";
            
            // Hücre referansını görüntüleme metni olarak kullanarak üçüncü bağlantıyı ekle
            int index3 = hyperlinks.Add("A3", 1, 1, "Sheet2!B5");
            hyperlinks[index3].TextToDisplay = "Go to Sheet2!B5";
            
            // Çalışma kitabını kaydedin
            string outputPath = "HyperlinkTextToDisplayDemo.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with hyperlinks using TextToDisplay property: " + outputPath);
        }
    }
}
```

### Ayrıca Bakınız

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


