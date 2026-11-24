---
title: "SmartTagCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SmartTagCollection-Eigenschaft. Gibt ein SmartTag‑Objekt am angegebenen Index zurück"
type: docs
url: /de/net/aspose.cells.markup/smarttagcollection/item/
---
## SmartTagCollection indexer

Ruft ein [`SmartTag`](../../smarttag/) Objekt am angegebenen Index ab

```csharp
public SmartTag this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index. |

### Rückgabewert

gibt ein [`SmartTag`](../../smarttag/) Objekt zurück.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Aspose");
            sheet.Cells["A2"].PutValue("Cells");

            SmartTagSetting smartTagSetting = sheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0);
            SmartTagCollection smartTags = smartTagSetting[smartTagIndex];

            smartTags.Add("http://docs.aspose.com", "docs");
            SmartTag smartTag = smartTags[0];
            smartTag.SetLink("http://www.aspose.com", "AsposeLink");

            SmartTagPropertyCollection properties = smartTag.Properties;
            properties.Add("Author", "Aspose");
            properties.Add("Description", "Aspose.Cells SmartTag");

            // Demonstriere die Verwendung der Item-Eigenschaft
            SmartTagProperty authorProperty = properties["Author"];
            Console.WriteLine($"Property 'Author' value: {authorProperty.Value}");

            workbook.Save("SmartTagPropertyDemo.xlsx");
            Console.WriteLine("SmartTagPropertyDemo.xlsx created successfully.");
        }
    }
}
```

### Siehe auch

* class [SmartTag](../../smarttag/)
* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


