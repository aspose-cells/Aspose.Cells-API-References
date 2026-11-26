---
title: "Clase XmlMap"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.XmlMap. Representa información del mapa Xml"
type: docs
url: /es/net/aspose.cells/xmlmap/
---
## XmlMap class

Representa la información del mapa Xml.

```csharp
public class XmlMap
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [DataBinding](../../aspose.cells/xmlmap/databinding/) { get; } | Obtiene un [`XmlDataBinding`](../xmldatabinding/) de este mapa. |
| [Name](../../aspose.cells/xmlmap/name/) { get; set; } | Devuelve o establece el nombre del objeto. |
| [RootElementName](../../aspose.cells/xmlmap/rootelementname/) { get; } | Obtiene el nombre del elemento raíz. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassXmlMapDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar datos de muestra a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Crear un mapa XML a partir de una cadena XML de ejemplo
            string xmlSchema = @"<xs:schema xmlns:xs='http://www.w3.org/2001/XMLSchema'>
                                <xs:element name='Data'>
                                    <xs:complexType>
                                        <xs:sequence>
                                            <xs:element name='Item' maxOccurs='unbounded'>
                                                <xs:complexType>
                                                    <xs:sequence>
                                                        <xs:element name='Name' type='xs:string'/>
                                                        <xs:element name='Value' type='xs:integer'/>
                                                    </xs:sequence>
                                                </xs:complexType>
                                            </xs:element>
                                        </xs:sequence>
                                    </xs:complexType>
                                </xs:element>
                            </xs:schema>";
            
            // Agregar el mapa XML al libro de trabajo
            int mapIndex = workbook.Worksheets.XmlMaps.Add(xmlSchema);
            XmlMap xmlMap = workbook.Worksheets.XmlMaps[mapIndex];
            
            // Exportar datos a XML usando el mapa
            workbook.ExportXml(xmlMap.Name, "output.xml");
            
            Console.WriteLine("XML exported successfully using XmlMap.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


