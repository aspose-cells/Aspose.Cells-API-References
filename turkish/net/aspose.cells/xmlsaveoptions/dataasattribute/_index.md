---
title: "XmlSaveOptions.DataAsAttribute"
second_title: "Aspose.Cells için .NET API Referansı"
description: "XmlSaveOptions özelliği. Verilerin öğenin öznitelikleri olarak dışa aktarılıp aktarılmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/xmlsaveoptions/dataasattribute/
---
## XmlSaveOptions.DataAsAttribute property

Verilerin öğenin öznitelikleri olarak dışa aktarılıp aktarılmayacağını gösterir.

```csharp
public bool DataAsAttribute { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertyDataAsAttributeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // DataAsAttribute true olarak ayarlanmış XML kaydetme seçeneklerini oluşturun
            XmlSaveOptions saveOptions = new XmlSaveOptions
            {
                DataAsAttribute = true,
                SheetNameAsElementName = true
            };

            // Verileri öznitelik olarak kaydet
            workbook.Save("DataAsAttribute_True.xml", saveOptions);

            // Verileri öğe olarak kaydetmek için değiştir
            saveOptions.DataAsAttribute = false;
            workbook.Save("DataAsAttribute_False.xml", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


