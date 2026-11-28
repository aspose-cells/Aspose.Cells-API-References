---
title: "XmlSaveOptions.XmlSaveOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "XmlSaveOptions yapıcı. XML dosyası kaydetmek için seçenekler oluşturur"
type: docs
url: /tr/net/aspose.cells/xmlsaveoptions/xmlsaveoptions/
---
## XmlSaveOptions constructor

Xml dosyasını kaydetmek için seçenekler oluşturur.

```csharp
public XmlSaveOptions()
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Test verileriyle örnek bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(63);

            // İlk demo: SheetNameAsElementName ile XML olarak kaydet
            XmlSaveOptions saveOptions1 = new XmlSaveOptions();
            saveOptions1.SheetNameAsElementName = true;
            workbook.Save("output1.xml", saveOptions1);
            
            // İkinci demo: SheetNameAsElementName ve DataAsAttribute ile XML olarak kaydet
            XmlSaveOptions saveOptions2 = new XmlSaveOptions();
            saveOptions2.SheetNameAsElementName = true;
            saveOptions2.DataAsAttribute = true;
            workbook.Save("output2.xml", saveOptions2);

            Console.WriteLine("XML files created successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


