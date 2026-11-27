---
title: "CustomXmlPart.SchemaData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CustomXmlPart‑egenskap. Hämtar eller anger XML‑innehållet för denna Custom XML Schema Data Storage Part"
type: docs
url: /sv/net/aspose.cells.markup/customxmlpart/schemadata/
---
## CustomXmlPart.SchemaData property

Hämtar eller sätter XML-innehållet för denna anpassade XML-schema datalagringsdel.

```csharp
public byte[] SchemaData { get; set; }
```

### Exempel

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

### Se även

* class [CustomXmlPart](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


