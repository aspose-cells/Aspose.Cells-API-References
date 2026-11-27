---
title: "XmlMapCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XmlMapCollection-egenskap. Hämtar xml‑kartan enligt det specifika indexet"
type: docs
url: /sv/net/aspose.cells/xmlmapcollection/item/
---
## XmlMapCollection indexer

Hämtar xml‑kartan efter det specifika indexet.

```csharp
public XmlMap this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Returvärde

Den xml‑kartan

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till XmlMapCollection från arbetsboken
            XmlMapCollection xmlMaps = workbook.Worksheets.XmlMaps;

            // Lägg till en ny XmlMap i samlingen
            int xmlMapIndex = xmlMaps.Add("data.xsd");

            // Åtkomst till XmlMap via Item‑egenskapen
            XmlMap xmlMap = xmlMaps[xmlMapIndex];

            // Visa XmlMap‑namnet
            Console.WriteLine("XmlMap Name: " + xmlMap.Name);

            // Spara arbetsboken
            workbook.Save("XmlMapCollectionExample.xlsx");
        }
    }
}
```

### Se även

* class [XmlMap](../../xmlmap/)
* class [XmlMapCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


