---
title: "Klasse VerticalPageBreakCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.VerticalPageBreakCollection Klasse. Kapselt eine Sammlung von VerticalPageBreak-Objekten"
type: docs
url: /de/net/aspose.cells/verticalpagebreakcollection/
---
## VerticalPageBreakCollection class

Kapselt eine Sammlung von [`VerticalPageBreak`](../verticalpagebreak/) Objekten.

```csharp
public class VerticalPageBreakCollection : CollectionBase<VerticalPageBreak>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/verticalpagebreakcollection/item/) { get; } | Ruft das [`VerticalPageBreak`](../verticalpagebreak/) Element am angegebenen Index ab. (2 Indexer) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells/verticalpagebreakcollection/add/#add)(int) | Fügt einen vertikalen Seitenumbruch zur Sammlung hinzu. |
| [Add](../../aspose.cells/verticalpagebreakcollection/add/#add_3)(string) | Fügt einen vertikalen Seitenumbruch zur Sammlung hinzu. |
| [Add](../../aspose.cells/verticalpagebreakcollection/add/#add_1)(int, int) | Fügt einen vertikalen Seitenumbruch zur Sammlung hinzu. |
| [Add](../../aspose.cells/verticalpagebreakcollection/add/#add_2)(int, int, int) | Fügt einen vertikalen Seitenumbruch zur Sammlung hinzu. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(VerticalPageBreak) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(VerticalPageBreak, IComparer&lt;VerticalPageBreak&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, VerticalPageBreak, IComparer&lt;VerticalPageBreak&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(VerticalPageBreak) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(VerticalPageBreak[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(VerticalPageBreak[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, VerticalPageBreak[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;VerticalPageBreak&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;VerticalPageBreak&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;VerticalPageBreak&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;VerticalPageBreak&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;VerticalPageBreak&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;VerticalPageBreak&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;VerticalPageBreak&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;VerticalPageBreak&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;VerticalPageBreak&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;VerticalPageBreak&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VerticalPageBreak) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VerticalPageBreak, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VerticalPageBreak, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VerticalPageBreak) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VerticalPageBreak, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VerticalPageBreak, int, int) |  |
| [RemoveAt](../../aspose.cells/verticalpagebreakcollection/removeat/#removeat)(int) | Entfernt das VPageBreak-Element bei einem angegebenen Namen. (2 Methoden) |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class VerticalPageBreakCollectionDemo
    {
        public static void VerticalPageBreakCollectionExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Zugriff auf die VerticalPageBreakCollection des Arbeitsblatts
            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;

            // Vertikale Seitenumbrüche hinzufügen
            verticalPageBreaks.Add(0, 10, 2); // From row 0 to 10 at column 2
            verticalPageBreaks.Add(4); // At column 4
            verticalPageBreaks.Add(5, 3); // At row 5, column 3
            verticalPageBreaks.Add("G5"); // At cell G5

            // Entferne einen vertikalen Seitenumbruch bei Index 1
            verticalPageBreaks.RemoveAt(1);

            // Zugriff und Ausgabe der Details der vertikalen Seitenumbrüche
            for (int i = 0; i < verticalPageBreaks.Count; i++)
            {
                VerticalPageBreak vpb = verticalPageBreaks[i];
                Console.WriteLine($"Vertical Page Break {i}: StartRow = {vpb.StartRow}, EndRow = {vpb.EndRow}, Column = {vpb.Column}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("VerticalPageBreakCollectionExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [VerticalPageBreak](../verticalpagebreak/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


