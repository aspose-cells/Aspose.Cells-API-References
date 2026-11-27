---
title: "Klass HyperlinkCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.HyperlinkCollection-klass. Inkapslar en samling av Hyperlink-objekt"
type: docs
url: /sv/net/aspose.cells/hyperlinkcollection/
---
## HyperlinkCollection class

Inkapslar en samling av [`Hyperlink`](../hyperlink/) objekt.

```csharp
public class HyperlinkCollection : CollectionBase<Hyperlink>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/hyperlinkcollection/item/) { get; } | Hämtar [`Hyperlink`](../hyperlink/) elementet på det angivna indexet. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells/hyperlinkcollection/add/#add_1)(string, int, int, string) | Lägger till en hyperlänk till en angiven cell eller ett cellområde. |
| [Add](../../aspose.cells/hyperlinkcollection/add/#add)(int, int, int, int, string) | Lägger till en hyperlänk till en angiven cell eller ett cellområde. |
| [Add](../../aspose.cells/hyperlinkcollection/add/#add_2)(string, string, string, string, string) | Lägger till en hyperlänk till en angiven cell eller ett cellområde. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Hyperlink) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Hyperlink, IComparer&lt;Hyperlink&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Hyperlink, IComparer&lt;Hyperlink&gt;) |  |
| [Clear](../../aspose.cells/hyperlinkcollection/clear/#clear)() | Rensar alla hyperlänkar. (2 metoder) |
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
| [RemoveAt](../../aspose.cells/hyperlinkcollection/removeat/#removeat)(int) | Ta bort hyperlänken på det angivna indexet i den här samlingen. (2 metoder) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HyperlinkCollectionDemo
    {
        public static void HyperlinkCollectionExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();

            // Hämtar referensen till det nyligen tillagda kalkylbladet genom att ange dess bladindex
            Worksheet worksheet = workbook.Worksheets[0];

            // Hämta samling av hyperlänkar
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;

            // Lägger till en hyperlänk till en URL i cellen "A1"
            hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

            // Lägger till en annan hyperlänk till en URL i cellen "B1"
            hyperlinks.Add("B1", 1, 1, "http://www.example.com");

            // Lägger till en hyperlänk med ett cellområde
            hyperlinks.Add("C1", 1, 2, "http://www.test.com");

            // Lägger till en hyperlänk med specifik visningstext och verktygstips
            hyperlinks.Add("D1", "D2", "http://www.display.com", "Click Here", "Go to Display");

            // Tar bort den första hyperlänken
            hyperlinks.RemoveAt(0);

            // Rensar alla hyperlänkar
            hyperlinks.Clear();

            // Lägger till en hyperlänk igen för att demonstrera sparande
            hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

            // Sparar Excel-filen
            workbook.Save("HyperlinkCollectionExample.xlsx");
            workbook.Save("HyperlinkCollectionExample.pdf");
            return;
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Hyperlink](../hyperlink/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


