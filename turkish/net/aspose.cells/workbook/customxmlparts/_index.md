---
title: "Workbook.CustomXmlParts"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook özelliği. Bir paket içinde Özel XML Veri Depolama Bölümü özel XML verisini temsil eder"
type: docs
url: /tr/net/aspose.cells/workbook/customxmlparts/
---
## Workbook.CustomXmlParts property

Özel bir XML Veri Depolama Bölümünü (paket içindeki özel XML verisi) temsil eder.

```csharp
public CustomXmlPartCollection CustomXmlParts { get; }
```

### Örnekler

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyCustomXmlPartsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            
            // XML verisini ve şemayı tanımla
            string xmlData = "<MyXmlData1 xmlns=\"http://my.namespace.com\"/>";
            string xmlSchema = "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>" +
                "<ds:datastoreItem ds:itemID=\"{1D3CF2F4-9155-40AE-99F6-33298D217F89}\" xmlns:ds=\"http://schemas.openxmlformats.org/officeDocument/2006/customXml\">" +
                    "<ds:schemaRefs>" +
                        "<ds:schemaRef ds:uri=\"http://my.namespace.com\"/>" +
                    "</ds:schemaRefs>" +
                "</ds:datastoreItem>";

            // Özel XML bölümünü Workbook'a ekle
            wb.CustomXmlParts.Add(Encoding.UTF8.GetBytes(xmlData), Encoding.UTF8.GetBytes(xmlSchema));

            // Workbook'ı kaydet ve yeniden yükle
            string outputPath = "output.xlsx";
            wb.Save(outputPath);
            
            Workbook loadedWb = new Workbook(outputPath);
            
            // Özel XML bölümlerinin sayısını göster
            Console.WriteLine($"Number of custom XML parts: {loadedWb.CustomXmlParts.Count}");
        }
    }
}
```

### Ayrıca Bakınız

* class [CustomXmlPartCollection](../../../aspose.cells.markup/customxmlpartcollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


