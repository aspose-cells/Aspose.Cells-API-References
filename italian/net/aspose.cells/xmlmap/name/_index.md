---
title: "XmlMap.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà XmlMap. Restituisce o imposta il nome dell'oggetto"
type: docs
url: /it/net/aspose.cells/xmlmap/name/
---
## XmlMap.Name property

Restituisce o imposta il nome dell'oggetto.

```csharp
public string Name { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapPropertyNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea dati di esempio
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("John Doe");
            
            // Aggiungi una mappa XML
            string xmlSchema = "<xs:schema xmlns:xs=\"http://www.w3.org/2001/XMLSchema\">" +
                "<xs:element name=\"Employee\">" +
                "<xs:complexType><xs:sequence>" +
                "<xs:element name=\"ID\" type=\"xs:int\"/>" +
                "<xs:element name=\"Name\" type=\"xs:string\"/>" +
                "</xs:sequence></xs:complexType></xs:element></xs:schema>";
                
            int mapIndex = workbook.Worksheets.XmlMaps.Add(xmlSchema);
            XmlMap map = workbook.Worksheets.XmlMaps[mapIndex];
            map.Name = "Employee";
            
            // Dimostra l'uso della proprietà Name
            Console.WriteLine("XML Map Name: " + map.Name);
            
            // Esporta in XML usando il nome della mappa
            string savePath = "output.xml";
            workbook.ExportXml(map.Name, savePath);
            
            Console.WriteLine("XML exported successfully to: " + savePath);
        }
    }
}
```

### Vedi anche

* class [XmlMap](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


