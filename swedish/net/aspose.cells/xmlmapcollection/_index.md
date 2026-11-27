---
title: "Klass XmlMapCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.XmlMapCollection-klass. En samling av XmlMap-objekt som representerar XmlMap-information"
type: docs
url: /sv/net/aspose.cells/xmlmapcollection/
---
## XmlMapCollection class

En samling av [`XmlMap`](../xmlmap/) objekt som representerar XmlMap-information.

```csharp
public class XmlMapCollection : CollectionBase<XmlMap>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/xmlmapcollection/item/) { get; } | Hämtar xml‑kartan efter det specifika indexet. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells/xmlmapcollection/add/)(string) | Lägg till en [`XmlMap`](../xmlmap/) via url/väg till en xml/xsd‑fil. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(XmlMap) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(XmlMap, IComparer&lt;XmlMap&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, XmlMap, IComparer&lt;XmlMap&gt;) |  |
| [Clear](../../aspose.cells/xmlmapcollection/clear/#clear)() | Tar bort alla XmlMaps. (2 metoder) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(XmlMap) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(XmlMap[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(XmlMap[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, XmlMap[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;XmlMap&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;XmlMap&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;XmlMap&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;XmlMap&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;XmlMap&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;XmlMap&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;XmlMap&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;XmlMap&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;XmlMap&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;XmlMap&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(XmlMap) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(XmlMap, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(XmlMap, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(XmlMap) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(XmlMap, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(XmlMap, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XmlMapCollectionDemo
    {
        public static void XmlMapCollectionExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till XmlMapCollection från arbetsboken
            XmlMapCollection xmlMaps = workbook.Worksheets.XmlMaps;

            // Lägg till en ny XmlMap i samlingen
            int xmlMapIndex = xmlMaps.Add("sample.xml");

            // Åtkomst till den nyligen tillagda XmlMap
            XmlMap xmlMap = xmlMaps[xmlMapIndex];

            // Visa antalet XmlMaps i samlingen
            Console.WriteLine("Number of XmlMaps: " + xmlMaps.Count);

            // Ange kapaciteten för XmlMapCollection
            xmlMaps.Capacity = 10;

            // Rensa alla XmlMaps från samlingen
            xmlMaps.Clear();

            // Spara arbetsboken
            workbook.Save("XmlMapCollectionExample.xlsx");

            return;
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [XmlMap](../xmlmap/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


