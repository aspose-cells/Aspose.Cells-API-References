---
title: "PasteOptions.IgnoreLinksToOriginalFile"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PasteOptions özelliği. Orijinal dosyaya bağlantıları yoksay"
type: docs
url: /tr/net/aspose.cells/pasteoptions/ignorelinkstooriginalfile/
---
## PasteOptions.IgnoreLinksToOriginalFile property

Orijinal dosyaya bağlantıları yok say.

```csharp
public bool IgnoreLinksToOriginalFile { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyIgnoreLinksToOriginalFileDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet src = workbook.Worksheets[0];
            
            // Orijinal dosyaya bağlanabilecek formüller içeren örnek veri oluştur
            src.Cells["A1"].PutValue("Header1");
            src.Cells["B1"].PutValue("Header2");
            src.Cells["A2"].PutValue(100);
            src.Cells["B2"].PutValue("=A2*2");  // Simple formula
            src.Cells["A3"].PutValue(200);
            src.Cells["B3"].PutValue("=A3*2");

            // Hedef çalışma sayfasını ve aralığı oluştur
            Worksheet dst = workbook.Worksheets.Add("Destination");
            Aspose.Cells.Range srcRange = src.Cells.CreateRange("A1:B3");
            Aspose.Cells.Range dstRange = dst.Cells.CreateRange("A1:B3");

            // Yapıştırma seçeneklerini orijinal dosyaya bağlantıları yoksayacak şekilde yapılandır
            PasteOptions pasteOptions = new PasteOptions();
            pasteOptions.PasteType = PasteType.All;
            pasteOptions.IgnoreLinksToOriginalFile = true;

            // Belirtilen yapıştırma seçenekleriyle kopyala
            dstRange.Copy(srcRange, pasteOptions);

            // Çalışma kitabını kaydedin
            workbook.Save("PasteOptions_IgnoreLinksToOriginalFile_Output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


