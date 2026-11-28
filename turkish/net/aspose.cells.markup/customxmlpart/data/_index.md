---
title: "CustomXmlPart.Data"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CustomXmlPart özelliği. Bu Custom XML Data Storage Part öğesinin XML içeriğini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.markup/customxmlpart/data/
---
## CustomXmlPart.Data property

Bu Özel XML Veri Depolama Bölümünün XML içeriğini alır veya ayarlar.

```csharp
public byte[] Data { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;
    using System.Text;

    public class CustomXmlPartPropertyDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            byte[] initialData = Encoding.UTF8.GetBytes("<root><data>Initial Value</data></root>");
            int xmlPartIndex = workbook.CustomXmlParts.Add(initialData, null);
            CustomXmlPart xmlPart = workbook.CustomXmlParts[xmlPartIndex];
            
            Console.WriteLine("Current Data value: " + Encoding.UTF8.GetString(xmlPart.Data));

            xmlPart.Data = Encoding.UTF8.GetBytes("<root><data>Modified Value</data></root>");

            workbook.CustomXmlParts.Add(xmlPart.Data, null);
            workbook.Save("CustomXmlPartDataDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CustomXmlPart](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


