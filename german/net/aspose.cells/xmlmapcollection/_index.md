---
title: "Klasse XmlMapCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.XmlMapCollection Klasse. Eine Sammlung von XmlMap‑Objekten, die XmlMap‑Informationen darstellen"
type: docs
url: /de/net/aspose.cells/xmlmapcollection/
---
## XmlMapCollection class

Eine Sammlung von [`XmlMap`](../xmlmap/) Objekten, die XmlMap‑Informationen darstellen.

```csharp
public class XmlMapCollection : CollectionBase<XmlMap>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/xmlmapcollection/item/) { get; } | Ruft die xml map anhand des angegebenen Index ab. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells/xmlmapcollection/add/)(string) | Fügen Sie ein [`XmlMap`](../xmlmap/) über die URL/Pfad einer xml/xsd‑Datei hinzu. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(XmlMap) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(XmlMap, IComparer&lt;XmlMap&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, XmlMap, IComparer&lt;XmlMap&gt;) |  |
| [Clear](../../aspose.cells/xmlmapcollection/clear/#clear)() | Entfernt alle XmlMaps. (2 Methoden) |
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

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XmlMapCollectionDemo
    {
        public static void XmlMapCollectionExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greifen Sie auf die XmlMapCollection aus der Arbeitsmappe zu
            XmlMapCollection xmlMaps = workbook.Worksheets.XmlMaps;

            // Fügen Sie ein neues XmlMap zur Sammlung hinzu
            int xmlMapIndex = xmlMaps.Add("sample.xml");

            // Zugriff auf die neu hinzugefügte XmlMap
            XmlMap xmlMap = xmlMaps[xmlMapIndex];

            // Anzeige der Anzahl von XmlMaps in der Sammlung
            Console.WriteLine("Number of XmlMaps: " + xmlMaps.Count);

            // Kapazität der XmlMapCollection festlegen
            xmlMaps.Capacity = 10;

            // Alle XmlMaps aus der Sammlung löschen
            xmlMaps.Clear();

            // Speichere die Arbeitsmappe
            workbook.Save("XmlMapCollectionExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [XmlMap](../xmlmap/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


