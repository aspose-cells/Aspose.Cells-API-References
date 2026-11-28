---
title: "Sınıf CustomXmlPart"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Markup.CustomXmlPart sınıfı. Bir paket içinde özel XML Veri Depolama Bölümü özel XML verisini temsil eder."
type: docs
url: /tr/net/aspose.cells.markup/customxmlpart/
---
## CustomXmlPart class

Özel bir XML Veri Depolama Bölümünü (paket içindeki özel XML verisi) temsil eder.

```csharp
public class CustomXmlPart
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Data](../../aspose.cells.markup/customxmlpart/data/) { get; set; } | Bu Özel XML Veri Depolama Bölümünün XML içeriğini alır veya ayarlar. |
| [ID](../../aspose.cells.markup/customxmlpart/id/) { get; set; } | Özel xml bölümünün kimliğini alır ve ayarlar. |
| [SchemaData](../../aspose.cells.markup/customxmlpart/schemadata/) { get; set; } | Bu Özel XML Şema Veri Depolama Bölümünün XML içeriğini alır veya ayarlar. |

### Örnekler

```csharp
using System;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class MarkupClassCustomXmlPartDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            CustomXmlPartCollection xmlParts = workbook.CustomXmlParts;

            string xmlData = "<root><item>Sample Data</item></root>";
            byte[] dataBytes = Encoding.UTF8.GetBytes(xmlData);

            string originalId = Guid.NewGuid().ToString();
            int index = xmlParts.Add(dataBytes, null);
            CustomXmlPart newPart = xmlParts[index];
            newPart.ID = originalId;

            Console.WriteLine("Original ID: " + originalId);
            Console.WriteLine("Stored ID: " + newPart.ID);

            string newId = Guid.NewGuid().ToString();
            newPart.ID = newId;
            Console.WriteLine("Updated ID: " + newId);

            workbook.Save("output.xlsx");

            Workbook loadedWorkbook = new Workbook("output.xlsx");
            CustomXmlPart retrievedPart = loadedWorkbook.CustomXmlParts.SelectByID(newId);
            Console.WriteLine("Retrieved ID: " + (retrievedPart != null ? retrievedPart.ID : "Not found"));
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


