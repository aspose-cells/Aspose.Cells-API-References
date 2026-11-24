---
title: "XmlMapCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "XmlMapCollection-Eigenschaft. Gibt die xml-Map anhand des angegebenen Index zurück."
type: docs
url: /de/net/aspose.cells/xmlmapcollection/item/
---
## XmlMapCollection indexer

Ruft die xml map anhand des angegebenen Index ab.

```csharp
public XmlMap this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index. |

### Rückgabewert

Die xml-Map.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greifen Sie auf die XmlMapCollection aus der Arbeitsmappe zu
            XmlMapCollection xmlMaps = workbook.Worksheets.XmlMaps;

            // Fügen Sie ein neues XmlMap zur Sammlung hinzu
            int xmlMapIndex = xmlMaps.Add("data.xsd");

            // Greifen Sie über die Item-Eigenschaft auf die XmlMap zu.
            XmlMap xmlMap = xmlMaps[xmlMapIndex];

            // Zeigen Sie den Namen der XmlMap an.
            Console.WriteLine("XmlMap Name: " + xmlMap.Name);

            // Speichere die Arbeitsmappe
            workbook.Save("XmlMapCollectionExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [XmlMap](../../xmlmap/)
* class [XmlMapCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


