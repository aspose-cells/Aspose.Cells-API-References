---
title: "CustomXmlPart.SchemaData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CustomXmlPart. تحصل أو تضبط محتوى XML لهذا الجزء المخصص لتخزين بيانات مخطط XML"
type: docs
url: /ar/net/aspose.cells.markup/customxmlpart/schemadata/
---
## CustomXmlPart.SchemaData property

يحصل أو يضبط محتوى XML لهذا Custom XML Schema Data Storage Part.

```csharp
public byte[] SchemaData { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;
    using System.Text;

    public class CustomXmlPartPropertySchemaDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            int index = workbook.CustomXmlParts.Add(null, null);
            CustomXmlPart customXmlPart = workbook.CustomXmlParts[index];
            Console.WriteLine("Current SchemaData: " + (customXmlPart.SchemaData == null ? "null" : Convert.ToBase64String(customXmlPart.SchemaData)));

            string schemaXml = "<?xml version=\"1.0\" encoding=\"UTF-8\"?><xs:schema xmlns:xs=\"http://www.w3.org/2001/XMLSchema\"><xs:element name=\"root\"/></xs:schema>";
            byte[] newSchemaData = Encoding.UTF8.GetBytes(schemaXml);
            customXmlPart.SchemaData = newSchemaData;

            Console.WriteLine("Updated SchemaData: " + Convert.ToBase64String(customXmlPart.SchemaData));

            workbook.Save("PropertySchemaDataDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CustomXmlPart](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


