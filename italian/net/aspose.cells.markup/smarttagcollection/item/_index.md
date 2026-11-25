---
title: "SmartTagCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SmartTagCollection. Ottiene un oggetto SmartTag all'indice specifico"
type: docs
url: /it/net/aspose.cells.markup/smarttagcollection/item/
---
## SmartTagCollection indexer

Ottiene un oggetto [`SmartTag`](../../smarttag/) all'indice specifico

```csharp
public SmartTag this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice. |

### Valore di ritorno

restituisce un oggetto [`SmartTag`](../../smarttag/).

### Esempi

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

            // Dimostra l'uso della proprietà Item
            SmartTagProperty authorProperty = properties["Author"];
            Console.WriteLine($"Property 'Author' value: {authorProperty.Value}");

            workbook.Save("SmartTagPropertyDemo.xlsx");
            Console.WriteLine("SmartTagPropertyDemo.xlsx created successfully.");
        }
    }
}
```

### Vedi anche

* class [SmartTag](../../smarttag/)
* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


