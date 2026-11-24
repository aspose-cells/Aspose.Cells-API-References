---
title: "XmlMapCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "XmlMapCollection-Methode. Fügt ein XmlMap über die URL/Pfad einer xml/xsd-Datei hinzu."
type: docs
url: /de/net/aspose.cells/xmlmapcollection/add/
---
## XmlMapCollection.Add method

Fügen Sie ein [`XmlMap`](../../xmlmap/) über die URL/Pfad einer xml/xsd-Datei hinzu.

```csharp
public int Add(string url)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| URL | String | URL/Pfad einer xml/xsd-Datei. |

### Rückgabewert

[`XmlMap`](../../xmlmap/) object index.

### Beispiele

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
            
            // Fügen Sie XML-Maps mithilfe von Schema- und XML-Dateien hinzu.
            xmlMapCollection.Add("schema.xsd");
            xmlMapCollection.Add("xml.xml");
            
            wb.Save("twoXmlMaps.xlsx");
        }
    }
}
```

### Siehe auch

* class [XmlMapCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


