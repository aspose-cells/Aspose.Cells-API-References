---
title: "XmlMap.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "XmlMap-Eigenschaft. Gibt den Namen des Objekts zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells/xmlmap/name/
---
## XmlMap.Name property

Gibt den Namen des Objekts zurück oder setzt ihn.

```csharp
public string Name { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapPropertyNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Arbeitsblatt hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle Beispieldaten
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("John Doe");
            
            // XML-Map hinzufügen
            string xmlSchema = "<xs:schema xmlns:xs=\"http://www.w3.org/2001/XMLSchema\">" +
                "<xs:element name=\"Employee\">" +
                "<xs:complexType><xs:sequence>" +
                "<xs:element name=\"ID\" type=\"xs:int\"/>" +
                "<xs:element name=\"Name\" type=\"xs:string\"/>" +
                "</xs:sequence></xs:complexType></xs:element></xs:schema>";
                
            int mapIndex = workbook.Worksheets.XmlMaps.Add(xmlSchema);
            XmlMap map = workbook.Worksheets.XmlMaps[mapIndex];
            map.Name = "Employee";
            
            // Verwendung der Name-Eigenschaft demonstrieren
            Console.WriteLine("XML Map Name: " + map.Name);
            
            // Export nach XML unter Verwendung des Namens der Map
            string savePath = "output.xml";
            workbook.ExportXml(map.Name, savePath);
            
            Console.WriteLine("XML exported successfully to: " + savePath);
        }
    }
}
```

### Siehe auch

* class [XmlMap](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


