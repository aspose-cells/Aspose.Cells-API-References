---
title: "WorksheetCollection.XmlMaps"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorksheetCollection. Obtiene y establece los mapas XML en el libro de trabajo"
type: docs
url: /es/net/aspose.cells/worksheetcollection/xmlmaps/
---
## WorksheetCollection.XmlMaps property

Obtiene y establece los mapas XML en el libro de trabajo.

```csharp
public XmlMapCollection XmlMaps { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyXmlMapsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar un mapa XML de ejemplo
            string xmlSchema = @"<xs:schema xmlns:xs='http://www.w3.org/2001/XMLSchema'>
                                <xs:element name='Root'>
                                    <xs:complexType>
                                        <xs:sequence>
                                            <xs:element name='Item' type='xs:string'/>
                                        </xs:sequence>
                                    </xs:complexType>
                                </xs:element>
                            </xs:schema>";
            
            // Agregar mapa XML al libro de trabajo
            int mapIndex = workbook.Worksheets.XmlMaps.Add(xmlSchema);
            
            // Acceder al mapa XML
            XmlMap map = workbook.Worksheets.XmlMaps[mapIndex];
            
            // Exportar datos XML (demuestra el uso de la propiedad XmlMaps)
            workbook.ExportXml(map.Name, "output.xml");
            
            Console.WriteLine("XML exported successfully using XmlMaps property.");
        }
    }
}
```

### Ver también

* class [XmlMapCollection](../../xmlmapcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


