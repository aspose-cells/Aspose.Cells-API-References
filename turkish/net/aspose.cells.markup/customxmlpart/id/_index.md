---
title: "CustomXmlPart.ID"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CustomXmlPart özelliği. Özel xml bölümünün kimliğini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.markup/customxmlpart/id/
---
## CustomXmlPart.ID property

Özel xml bölümünün kimliğini alır ve ayarlar.

```csharp
public string ID { get; set; }
```

### Örnekler

```csharp
using System;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class CustomXmlPartPropertyIDDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            int partIndex = workbook.CustomXmlParts.Add(
                Encoding.UTF8.GetBytes("<root><data>Sample</data></root>"), 
                null);
            CustomXmlPart part = workbook.CustomXmlParts[partIndex];
            
            string originalId = "2F087CB2-7CA8-43DA-B048-2E2F61F4936F";
            part.ID = originalId;
            workbook.Save("CustomXmlPartDemo.xlsx");

            Workbook reloadedWorkbook = new Workbook("CustomXmlPartDemo.xlsx");
            CustomXmlPart reloadedPart = reloadedWorkbook.CustomXmlParts.SelectByID(originalId);
            Console.WriteLine("Original ID: " + reloadedPart.ID);

            string newId = "2F087CB2-7CA8-43DA-B048-2E2F61F0000F";
            reloadedPart.ID = newId;
            reloadedWorkbook.Save("CustomXmlPartDemo_Updated.xlsx");

            Workbook finalWorkbook = new Workbook("CustomXmlPartDemo_Updated.xlsx");
            CustomXmlPart finalPart = finalWorkbook.CustomXmlParts.SelectByID(newId);
            Console.WriteLine("New ID: " + finalPart.ID);
        }
    }
}
```

### Ayrıca Bakınız

* class [CustomXmlPart](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


