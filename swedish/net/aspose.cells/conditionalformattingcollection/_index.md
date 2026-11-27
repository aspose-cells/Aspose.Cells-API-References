---
title: "Klass ConditionalFormattingCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ConditionalFormattingCollection klass. Inkapslar en samling av FormatCondition-objekt"
type: docs
url: /sv/net/aspose.cells/conditionalformattingcollection/
---
## ConditionalFormattingCollection class

Inkapslar en samling av [`FormatCondition`](../formatcondition/) objekt.

```csharp
public class ConditionalFormattingCollection : CollectionBase<FormatConditionCollection>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/conditionalformattingcollection/item/) { get; } | Hämtar FormatConditions-elementet på det angivna indexet. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells/conditionalformattingcollection/add/)() | Lägger till en FormatConditions i samlingen. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(FormatConditionCollection) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(FormatConditionCollection, IComparer&lt;FormatConditionCollection&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, FormatConditionCollection, IComparer&lt;FormatConditionCollection&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(FormatConditionCollection) |  |
| [Copy](../../aspose.cells/conditionalformattingcollection/copy/)(ConditionalFormattingCollection) | Kopierar villkorlig formatering. |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(FormatConditionCollection[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(FormatConditionCollection[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, FormatConditionCollection[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FormatConditionCollection) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FormatConditionCollection, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FormatConditionCollection, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FormatConditionCollection) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FormatConditionCollection, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FormatConditionCollection, int, int) |  |
| [RemoveArea](../../aspose.cells/conditionalformattingcollection/removearea/)(int, int, int, int) | Ta bort all villkorlig formatering i intervallet. |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ConditionalFormattingCollectionDemo
    {
        public static void ConditionalFormattingCollectionExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Hämta villkorlig formatering
            ConditionalFormattingCollection cformattings = sheet.ConditionalFormattings;

            // Lägger till en tom villkorlig formatering
            int index = cformattings.Add();

            // Hämta nyss tillagd villkorlig formatering
            FormatConditionCollection fcs = cformattings[index];

            // Ställer in det villkorsstyrda formatintervallet.
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 0,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            ca = new CellArea
            {
                StartRow = 1,
                EndRow = 1,
                StartColumn = 1,
                EndColumn = 1
            };
            fcs.AddArea(ca);

            // Lägg till villkor.
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");

            // Ställer in bakgrundsfärgen.
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            // Sparar Excel-filen
            workbook.Save("ConditionalFormattingCollectionDemo.xlsx");
            workbook.Save("ConditionalFormattingCollectionDemo.pdf");
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [FormatConditionCollection](../formatconditioncollection/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


