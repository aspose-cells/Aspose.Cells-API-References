---
title: "الفئة XmlMap"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.XmlMap. تمثل معلومات خريطة Xml"
type: docs
url: /ar/net/aspose.cells/xmlmap/
---
## XmlMap class

يمثل معلومات خريطة Xml.

```csharp
public class XmlMap
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [DataBinding](../../aspose.cells/xmlmap/databinding/) { get; } | تحصل على [`XmlDataBinding`](../xmldatabinding/) لهذه الخريطة. |
| [Name](../../aspose.cells/xmlmap/name/) { get; set; } | إرجاع أو تعيين اسم الكائن. |
| [RootElementName](../../aspose.cells/xmlmap/rootelementname/) { get; } | تحصل على اسم العنصر الجذر. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassXmlMapDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة بيانات نموذجية إلى الورقة الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // إنشاء خريطة XML من سلسلة XML نموذجية
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
            
            // إضافة خريطة XML إلى المصنف
            int mapIndex = workbook.Worksheets.XmlMaps.Add(xmlSchema);
            XmlMap xmlMap = workbook.Worksheets.XmlMaps[mapIndex];
            
            // تصدير البيانات إلى XML باستخدام الخريطة
            workbook.ExportXml(xmlMap.Name, "output.xml");
            
            Console.WriteLine("XML exported successfully using XmlMap.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


