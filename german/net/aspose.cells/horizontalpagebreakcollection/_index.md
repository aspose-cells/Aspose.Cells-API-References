---
title: "Class HorizontalPageBreakCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.HorizontalPageBreakCollection Klasse. Kapselt eine Sammlung von HorizontalPageBreak-Objekten"
type: docs
url: /de/net/aspose.cells/horizontalpagebreakcollection/
---
## HorizontalPageBreakCollection class

Kapselt eine Sammlung von [`HorizontalPageBreak`](../horizontalpagebreak/) Objekten.

```csharp
public class HorizontalPageBreakCollection : CollectionBase<HorizontalPageBreak>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/horizontalpagebreakcollection/item/) { get; } | Liefert das [`HorizontalPageBreak`](../horizontalpagebreak/) Element am angegebenen Index. (2 Indexer) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells/horizontalpagebreakcollection/add/#add)(int) | Fügt der Sammlung einen horizontalen Seitenumbruch hinzu. |
| [Add](../../aspose.cells/horizontalpagebreakcollection/add/#add_3)(string) | Fügt der Sammlung einen horizontalen Seitenumbruch hinzu. |
| [Add](../../aspose.cells/horizontalpagebreakcollection/add/#add_1)(int, int) | Fügt der Sammlung einen horizontalen Seitenumbruch hinzu. |
| [Add](../../aspose.cells/horizontalpagebreakcollection/add/#add_2)(int, int, int) | Fügt der Sammlung einen horizontalen Seitenumbruch hinzu. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(HorizontalPageBreak) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(HorizontalPageBreak, IComparer&lt;HorizontalPageBreak&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, HorizontalPageBreak, IComparer&lt;HorizontalPageBreak&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(HorizontalPageBreak) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(HorizontalPageBreak[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(HorizontalPageBreak[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, HorizontalPageBreak[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;HorizontalPageBreak&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;HorizontalPageBreak&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HorizontalPageBreak) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HorizontalPageBreak, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HorizontalPageBreak, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HorizontalPageBreak) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HorizontalPageBreak, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HorizontalPageBreak, int, int) |  |
| [RemoveAt](../../aspose.cells/horizontalpagebreakcollection/removeat/#removeat)(int) | Entfernt das HPageBreak-Element mit einem angegebenen Namen. (2 Methoden) |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HorizontalPageBreakCollectionDemo
    {
        public static void HorizontalPageBreakCollectionExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge einen horizontalen Seitenumbruch in Zeile 5 ein
            worksheet.HorizontalPageBreaks.Add(5);
            
            // Füge einen horizontalen Seitenumbruch in Zeile 10 ein, beginnend bei Spalte 1 bis Spalte 5
            worksheet.HorizontalPageBreaks.Add(10, 1, 5);
            
            // Füge einen horizontalen Seitenumbruch in Zeile 15 ein, beginnend bei Spalte 2
            worksheet.HorizontalPageBreaks.Add(15, 2);
            
            // Füge einen horizontalen Seitenumbruch in Zelle "G5" ein
            worksheet.HorizontalPageBreaks.Add("G5");
            
            // Entferne den ersten horizontalen Seitenumbruch
            worksheet.HorizontalPageBreaks.RemoveAt(0);
            
            // Speichere die Arbeitsmappe
            workbook.Save("HorizontalPageBreakCollectionExample.xlsx");
            workbook.Save("HorizontalPageBreakCollectionExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [HorizontalPageBreak](../horizontalpagebreak/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


