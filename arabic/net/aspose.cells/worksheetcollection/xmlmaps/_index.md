---
title: "WorksheetCollection.XmlMaps"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorksheetCollection. تحصل وتعيّن خرائط XML في المصنف"
type: docs
url: /ar/net/aspose.cells/worksheetcollection/xmlmaps/
---
## WorksheetCollection.XmlMaps property

يحصل على ويضبط خرائط XML في المصنف.

```csharp
public XmlMapCollection XmlMaps { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyXmlMapsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة خريطة XML نموذجية
            string xmlSchema = @"<xs:schema xmlns:xs='http://www.w3.org/2001/XMLSchema'>
                                <xs:element name='Root'>
                                    <xs:complexType>
                                        <xs:sequence>
                                            <xs:element name='Item' type='xs:string'/>
                                        </xs:sequence>
                                    </xs:complexType>
                                </xs:element>
                            </xs:schema>";
            
            // إضافة خريطة XML إلى المصنف
            int mapIndex = workbook.Worksheets.XmlMaps.Add(xmlSchema);
            
            // الوصول إلى خريطة XML
            XmlMap map = workbook.Worksheets.XmlMaps[mapIndex];
            
            // تصدير بيانات XML (يوضح استخدام خاصية XmlMaps)
            workbook.ExportXml(map.Name, "output.xml");
            
            Console.WriteLine("XML exported successfully using XmlMaps property.");
        }
    }
}
```

### انظر أيضًا

* class [XmlMapCollection](../../xmlmapcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


