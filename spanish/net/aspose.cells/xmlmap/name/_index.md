---
title: "XmlMap.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad XmlMap. Devuelve o establece el nombre del objeto"
type: docs
url: /es/net/aspose.cells/xmlmap/name/
---
## XmlMap.Name property

Devuelve o establece el nombre del objeto.

```csharp
public string Name { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapPropertyNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear datos de ejemplo
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("John Doe");
            
            // Agregar un mapa XML
            string xmlSchema = "<xs:schema xmlns:xs=\"http://www.w3.org/2001/XMLSchema\">" +
                "<xs:element name=\"Employee\">" +
                "<xs:complexType><xs:sequence>" +
                "<xs:element name=\"ID\" type=\"xs:int\"/>" +
                "<xs:element name=\"Name\" type=\"xs:string\"/>" +
                "</xs:sequence></xs:complexType></xs:element></xs:schema>";
                
            int mapIndex = workbook.Worksheets.XmlMaps.Add(xmlSchema);
            XmlMap map = workbook.Worksheets.XmlMaps[mapIndex];
            map.Name = "Employee";
            
            // Demostrar el uso de la propiedad Name
            Console.WriteLine("XML Map Name: " + map.Name);
            
            // Exportar a XML usando el nombre del mapa
            string savePath = "output.xml";
            workbook.ExportXml(map.Name, savePath);
            
            Console.WriteLine("XML exported successfully to: " + savePath);
        }
    }
}
```

### Ver también

* class [XmlMap](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


