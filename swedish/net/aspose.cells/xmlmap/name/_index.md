---
title: "XmlMap.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XmlMap‑egenskap. Returnerar eller anger namn på objektet"
type: docs
url: /sv/net/aspose.cells/xmlmap/name/
---
## XmlMap.Name property

Returnerar eller anger namnet på objektet.

```csharp
public string Name { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapPropertyNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa exempeldata
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("John Doe");
            
            // Lägg till en XML‑karta
            string xmlSchema = "<xs:schema xmlns:xs=\"http://www.w3.org/2001/XMLSchema\">" +
                "<xs:element name=\"Employee\">" +
                "<xs:complexType><xs:sequence>" +
                "<xs:element name=\"ID\" type=\"xs:int\"/>" +
                "<xs:element name=\"Name\" type=\"xs:string\"/>" +
                "</xs:sequence></xs:complexType></xs:element></xs:schema>";
                
            int mapIndex = workbook.Worksheets.XmlMaps.Add(xmlSchema);
            XmlMap map = workbook.Worksheets.XmlMaps[mapIndex];
            map.Name = "Employee";
            
            // Demonstrera användning av Name‑egenskapen
            Console.WriteLine("XML Map Name: " + map.Name);
            
            // Exportera till XML med kartans namn
            string savePath = "output.xml";
            workbook.ExportXml(map.Name, savePath);
            
            Console.WriteLine("XML exported successfully to: " + savePath);
        }
    }
}
```

### Se även

* class [XmlMap](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


