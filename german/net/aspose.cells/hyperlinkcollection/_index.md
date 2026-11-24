---
title: "Klasse HyperlinkCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.HyperlinkCollection Klasse. Kapselt eine Sammlung von Hyperlink-Objekten"
type: docs
url: /de/net/aspose.cells/hyperlinkcollection/
---
## HyperlinkCollection class

Kapselt eine Sammlung von [`Hyperlink`](../hyperlink/) Objekten.

```csharp
public class HyperlinkCollection : CollectionBase<Hyperlink>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/hyperlinkcollection/item/) { get; } | Liest das [`Hyperlink`](../hyperlink/) Element am angegebenen Index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells/hyperlinkcollection/add/#add_1)(string, int, int, string) | Fügt einen Hyperlink zu einer angegebenen Zelle oder einem Zellbereich hinzu. |
| [Add](../../aspose.cells/hyperlinkcollection/add/#add)(int, int, int, int, string) | Fügt einen Hyperlink zu einer angegebenen Zelle oder einem Zellbereich hinzu. |
| [Add](../../aspose.cells/hyperlinkcollection/add/#add_2)(string, string, string, string, string) | Fügt einen Hyperlink zu einer angegebenen Zelle oder einem Zellbereich hinzu. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Hyperlink) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Hyperlink, IComparer&lt;Hyperlink&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Hyperlink, IComparer&lt;Hyperlink&gt;) |  |
| [Clear](../../aspose.cells/hyperlinkcollection/clear/#clear)() | Löscht alle Hyperlinks. (2 Methoden) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Hyperlink) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Hyperlink[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Hyperlink[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Hyperlink[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Hyperlink&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Hyperlink&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Hyperlink&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Hyperlink&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Hyperlink&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Hyperlink) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Hyperlink, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Hyperlink, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Hyperlink) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Hyperlink, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Hyperlink, int, int) |  |
| [RemoveAt](../../aspose.cells/hyperlinkcollection/removeat/#removeat)(int) | Entfernt den Hyperlink am angegebenen Index in dieser Sammlung. (2 Methoden) |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HyperlinkCollectionDemo
    {
        public static void HyperlinkCollectionExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();

            // Abrufen der Referenz des neu hinzugefügten Arbeitsblatts durch Übergabe seines Blattindexes
            Worksheet worksheet = workbook.Worksheets[0];

            // Hyperlink-Sammlung abrufen
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;

            // Hinzufügen eines Hyperlinks zu einer URL in Zelle "A1"
            hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

            // Hinzufügen eines weiteren Hyperlinks zu einer URL in Zelle "B1"
            hyperlinks.Add("B1", 1, 1, "http://www.example.com");

            // Hinzufügen eines Hyperlinks mit einem Zellbereich
            hyperlinks.Add("C1", 1, 2, "http://www.test.com");

            // Hinzufügen eines Hyperlinks mit einem bestimmten Anzeigetext und Bildschirmhinweis
            hyperlinks.Add("D1", "D2", "http://www.display.com", "Click Here", "Go to Display");

            // Entfernen des ersten Hyperlinks
            hyperlinks.RemoveAt(0);

            // Alle Hyperlinks löschen
            hyperlinks.Clear();

            // Erneutes Hinzufügen eines Hyperlinks, um das Speichern zu demonstrieren
            hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

            // Die Excel-Datei speichern
            workbook.Save("HyperlinkCollectionExample.xlsx");
            workbook.Save("HyperlinkCollectionExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Hyperlink](../hyperlink/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


