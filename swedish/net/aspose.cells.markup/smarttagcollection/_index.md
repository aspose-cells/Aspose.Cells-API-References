---
title: "Klass SmartTagCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Markup.SmartTagCollection-klass. Representerar alla smarta taggar i cellen"
type: docs
url: /sv/net/aspose.cells.markup/smarttagcollection/
---
## SmartTagCollection class

Representerar alla smarta taggar i cellen.

```csharp
public class SmartTagCollection : CollectionBase<SmartTag>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Column](../../aspose.cells.markup/smarttagcollection/column/) { get; } | Hämtar kolumnen för cellens smarta taggar. |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.markup/smarttagcollection/item/) { get; } | Hämtar ett [`SmartTag`](../smarttag/) objekt på det specifika indexet |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [Row](../../aspose.cells.markup/smarttagcollection/row/) { get; } | Hämtar raden för cellens smarta taggar. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells.markup/smarttagcollection/add/)(string, string) | Lägger till en smart tagg. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(SmartTag) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(SmartTag, IComparer&lt;SmartTag&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, SmartTag, IComparer&lt;SmartTag&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(SmartTag) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(SmartTag[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(SmartTag[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, SmartTag[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;SmartTag&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;SmartTag&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;SmartTag&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;SmartTag&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;SmartTag&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;SmartTag&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;SmartTag&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;SmartTag&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;SmartTag&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;SmartTag&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SmartTag) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SmartTag, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SmartTag, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SmartTag) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SmartTag, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SmartTag, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class MarkupClassSmartTagCollectionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            smartTagSetting.Add(0, 0); // Add smart tag to cell A1

            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
            smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            Console.WriteLine("Smart Tags Count: " + smartTagSetting.Count);
            workbook.Save("SmartTagCollectionDemo.xlsx");
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [SmartTag](../smarttag/)
* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


