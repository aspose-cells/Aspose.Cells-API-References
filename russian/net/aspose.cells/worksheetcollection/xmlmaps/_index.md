---
title: "WorksheetCollection.XmlMaps"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorksheetCollection. Получает и задает XML-карты в рабочей книге"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/xmlmaps/
---
## WorksheetCollection.XmlMaps property

Получает и задает XML‑карты в книге.

```csharp
public XmlMapCollection XmlMaps { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyXmlMapsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить пример XML-карты
            string xmlSchema = @"<xs:schema xmlns:xs='http://www.w3.org/2001/XMLSchema'>
                                <xs:element name='Root'>
                                    <xs:complexType>
                                        <xs:sequence>
                                            <xs:element name='Item' type='xs:string'/>
                                        </xs:sequence>
                                    </xs:complexType>
                                </xs:element>
                            </xs:schema>";
            
            // Добавить XML-карту в рабочую книгу
            int mapIndex = workbook.Worksheets.XmlMaps.Add(xmlSchema);
            
            // Получить доступ к XML-карте
            XmlMap map = workbook.Worksheets.XmlMaps[mapIndex];
            
            // Экспорт данных XML (демонстрирует использование свойства XmlMaps)
            workbook.ExportXml(map.Name, "output.xml");
            
            Console.WriteLine("XML exported successfully using XmlMaps property.");
        }
    }
}
```

### См. также

* class [XmlMapCollection](../../xmlmapcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


