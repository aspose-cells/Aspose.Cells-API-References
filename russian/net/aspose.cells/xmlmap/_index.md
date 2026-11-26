---
title: "Класс XmlMap"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.XmlMap. Представляет информацию о XML‑карте"
type: docs
url: /ru/net/aspose.cells/xmlmap/
---
## XmlMap class

Представляет информацию о карте Xml.

```csharp
public class XmlMap
```

## Свойства

| Имя | Описание |
| --- | --- |
| [DataBinding](../../aspose.cells/xmlmap/databinding/) { get; } | Получает [`XmlDataBinding`](../xmldatabinding/) этой карты. |
| [Name](../../aspose.cells/xmlmap/name/) { get; set; } | Возвращает или задает имя объекта. |
| [RootElementName](../../aspose.cells/xmlmap/rootelementname/) { get; } | Получает имя корневого элемента. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassXmlMapDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте примерные данные в первый лист
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Создать XML‑карту из образца XML‑строки
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
            
            // Добавить XML‑карту в книгу
            int mapIndex = workbook.Worksheets.XmlMaps.Add(xmlSchema);
            XmlMap xmlMap = workbook.Worksheets.XmlMaps[mapIndex];
            
            // Экспортировать данные в XML с использованием карты
            workbook.ExportXml(xmlMap.Name, "output.xml");
            
            Console.WriteLine("XML exported successfully using XmlMap.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


