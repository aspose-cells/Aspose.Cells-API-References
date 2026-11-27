---
title: "XmlMap.RootElementName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XmlMap‑egenskap. Hämtar rot-elementets namn"
type: docs
url: /sv/net/aspose.cells/xmlmap/rootelementname/
---
## XmlMap.RootElementName property

Hämtar rot-elementets namn.

```csharp
public string RootElementName { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapPropertyRootElementNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);

            // Skapa en XML‑karta
            string xml = "<root><item><Name>Item1</Name><Value>100</Value></item></root>";
            int mapIndex = workbook.Worksheets.XmlMaps.Add(xml);
            
            // Hämta och visa rot-elementets namn
            string rootElementName = workbook.Worksheets.XmlMaps[mapIndex].RootElementName;
            Console.WriteLine("Root Element Name: " + rootElementName);
        }
    }
}
```

### Se även

* class [XmlMap](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


