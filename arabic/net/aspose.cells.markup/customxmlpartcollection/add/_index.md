---
title: "CustomXmlPartCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CustomXmlPartCollection. تضيف عنصرًا إلى المجموعة"
type: docs
url: /ar/net/aspose.cells.markup/customxmlpartcollection/add/
---
## CustomXmlPartCollection.Add method

يضيف عنصرًا إلى المجموعة.

```csharp
public int Add(byte[] data, byte[] schemaData)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| بيانات | Byte[] | محتوى XML لهذا الجزء المخصص لتخزين البيانات |
| schemaData | Byte[] | مجموعة مخططات XML المرتبطة بهذا الجزء المخصص من XML |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;
    using System.Text;

    public class CustomXmlPartCollectionMethodAddWithByteByteDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // احصل على CustomXmlPartCollection مباشرةً من المصنف
            CustomXmlPartCollection customXmlParts = workbook.CustomXmlParts;
            
            // جهّز بيانات XML والمخطط كمصفوفات بايت
            string xmlData = "<root><item>Test Data</item></root>";
            string schemaData = "<xs:schema xmlns:xs='http://www.w3.org/2001/XMLSchema'><xs:element name='root'><xs:complexType><xs:sequence><xs:element name='item' type='xs:string'/></xs:sequence></xs:complexType></xs:element></xs:schema>";
            
            byte[] xmlBytes = Encoding.UTF8.GetBytes(xmlData);
            byte[] schemaBytes = Encoding.UTF8.GetBytes(schemaData);

            try
            {
                // استدعِ طريقة Add مع معلمات مصفوفة البايت
                int index = customXmlParts.Add(xmlBytes, schemaBytes);
                
                Console.WriteLine($"Custom XML part added successfully at index: {index}");
                
                // احفظ المصنف لتوضيح التأثير
                workbook.Save("CustomXmlPartAddDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding custom XML part: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [CustomXmlPartCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


