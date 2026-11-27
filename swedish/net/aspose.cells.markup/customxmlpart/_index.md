---
title: "Klass CustomXmlPart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Markup.CustomXmlPart‑klass. Representerar en Custom XML Data Storage Part‑del med anpassad XML‑data inom ett paket"
type: docs
url: /sv/net/aspose.cells.markup/customxmlpart/
---
## CustomXmlPart class

Representerar en anpassad XML‑databasdel (anpassad XML‑data inom ett paket).

```csharp
public class CustomXmlPart
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Data](../../aspose.cells.markup/customxmlpart/data/) { get; set; } | Hämtar eller anger XML‑innehållet för denna Custom XML Data Storage Part. |
| [ID](../../aspose.cells.markup/customxmlpart/id/) { get; set; } | Hämtar och sätter id för den anpassade xml-delen. |
| [SchemaData](../../aspose.cells.markup/customxmlpart/schemadata/) { get; set; } | Hämtar eller sätter XML-innehållet för denna anpassade XML-schema datalagringsdel. |

### Exempel

```csharp
using System;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class MarkupClassCustomXmlPartDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            CustomXmlPartCollection xmlParts = workbook.CustomXmlParts;

            string xmlData = "<root><item>Sample Data</item></root>";
            byte[] dataBytes = Encoding.UTF8.GetBytes(xmlData);

            string originalId = Guid.NewGuid().ToString();
            int index = xmlParts.Add(dataBytes, null);
            CustomXmlPart newPart = xmlParts[index];
            newPart.ID = originalId;

            Console.WriteLine("Original ID: " + originalId);
            Console.WriteLine("Stored ID: " + newPart.ID);

            string newId = Guid.NewGuid().ToString();
            newPart.ID = newId;
            Console.WriteLine("Updated ID: " + newId);

            workbook.Save("output.xlsx");

            Workbook loadedWorkbook = new Workbook("output.xlsx");
            CustomXmlPart retrievedPart = loadedWorkbook.CustomXmlParts.SelectByID(newId);
            Console.WriteLine("Retrieved ID: " + (retrievedPart != null ? retrievedPart.ID : "Not found"));
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


