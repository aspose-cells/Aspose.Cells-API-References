---
title: "XmlSaveOptions.XmlMapName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "XmlSaveOptions özelliği. Dosyada xml haritasının dışa aktarılıp aktarılmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells/xmlsaveoptions/xmlmapname/
---
## XmlSaveOptions.XmlMapName property

Dosyada xml haritasının dışa aktarılıp aktarılmayacağını gösterir.

```csharp
public string XmlMapName { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertyXmlMapNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı verileri doldurun
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);

            // XML haritası oluştur ve çalışma kitabına ekle
            int mapIndex = workbook.Worksheets.XmlMaps.Add("<Schema><Element><Product/><Price/></Element></Schema>");
            XmlMap xmlMap = workbook.Worksheets.XmlMaps[mapIndex];
            xmlMap.Name = "ProductDataMap";

            // XmlSaveOptions oluşturun ve XmlMapName'i ayarlayın
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.XmlMapName = "ProductDataMap";

            // Çalışma kitabını XML haritalama ile kaydedin
            workbook.Save("XmlWithMapping.xml", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


