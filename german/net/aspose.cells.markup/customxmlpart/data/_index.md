---
title: "CustomXmlPart.Data"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CustomXmlPart property. Gibt den XML‑Inhalt dieses benutzerdefinierten XML‑Datenspeicher‑Teils zurück oder setzt ihn."
type: docs
url: /de/net/aspose.cells.markup/customxmlpart/data/
---
## CustomXmlPart.Data property

Liest oder legt den XML-Inhalt dieses Custom XML Data Storage Part fest.

```csharp
public byte[] Data { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;
    using System.Text;

    public class CustomXmlPartPropertyDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            byte[] initialData = Encoding.UTF8.GetBytes("<root><data>Initial Value</data></root>");
            int xmlPartIndex = workbook.CustomXmlParts.Add(initialData, null);
            CustomXmlPart xmlPart = workbook.CustomXmlParts[xmlPartIndex];
            
            Console.WriteLine("Current Data value: " + Encoding.UTF8.GetString(xmlPart.Data));

            xmlPart.Data = Encoding.UTF8.GetBytes("<root><data>Modified Value</data></root>");

            workbook.CustomXmlParts.Add(xmlPart.Data, null);
            workbook.Save("CustomXmlPartDataDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CustomXmlPart](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


