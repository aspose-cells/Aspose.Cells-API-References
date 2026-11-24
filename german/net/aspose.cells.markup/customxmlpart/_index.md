---
title: "Klasse CustomXmlPart"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Markup.CustomXmlPart class. Stellt einen Custom XML Data Storage Part mit benutzerdefinierten XML-Daten innerhalb eines Pakets dar"
type: docs
url: /de/net/aspose.cells.markup/customxmlpart/
---
## CustomXmlPart class

Stellt einen benutzerdefinierten XML‑Datenspeicherteil dar (benutzerdefinierte XML‑Daten innerhalb eines Pakets).

```csharp
public class CustomXmlPart
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Data](../../aspose.cells.markup/customxmlpart/data/) { get; set; } | Liest oder legt den XML-Inhalt dieses Custom XML Data Storage Part fest. |
| [ID](../../aspose.cells.markup/customxmlpart/id/) { get; set; } | Liest und legt die ID des custom xml part fest. |
| [SchemaData](../../aspose.cells.markup/customxmlpart/schemadata/) { get; set; } | Liest oder legt den XML-Inhalt dieses Custom XML Schema Data Storage Part fest. |

### Beispiele

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

### Siehe auch

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


