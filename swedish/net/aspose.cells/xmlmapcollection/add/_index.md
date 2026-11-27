---
title: "XmlMapCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XmlMapCollection-metod. Lägg till en XmlMap via url/sökväg för en xml/xsd-fil"
type: docs
url: /sv/net/aspose.cells/xmlmapcollection/add/
---
## XmlMapCollection.Add method

Lägg till en [`XmlMap`](../../xmlmap/) via url/sökväg för en xml/xsd-fil.

```csharp
public int Add(string url)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| url | String | url/sökväg för en xml/xsd-fil. |

### Returvärde

[`XmlMap`](../../xmlmap/) object index.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            
            XmlMapCollection xmlMapCollection = wb.Worksheets.XmlMaps;
            
            // Lägg till XML-kartor med hjälp av schema- och XML-filer
            xmlMapCollection.Add("schema.xsd");
            xmlMapCollection.Add("xml.xml");
            
            wb.Save("twoXmlMaps.xlsx");
        }
    }
}
```

### Se även

* class [XmlMapCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


