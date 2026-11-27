---
title: "Klass ConditionalFormattingValueCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ConditionalFormattingValueCollection-klass. Beskriver en samling av CFValueObject. Använd endast för ikonsätt"
type: docs
url: /sv/net/aspose.cells/conditionalformattingvaluecollection/
---
## ConditionalFormattingValueCollection class

Beskriver en samling av CFValueObject. Använd endast för ikonsatser.

```csharp
public class ConditionalFormattingValueCollection : CollectionBase<ConditionalFormattingValue>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/conditionalformattingvaluecollection/item/) { get; } | Hämta CFValueObject-elementet på det angivna indexet. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells/conditionalformattingvaluecollection/add/)(FormatConditionValueType, string) | Lägger till [`ConditionalFormattingValue`](../conditionalformattingvalue/) objekt. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ConditionalFormattingValue) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ConditionalFormattingValue, IComparer&lt;ConditionalFormattingValue&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ConditionalFormattingValue, IComparer&lt;ConditionalFormattingValue&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ConditionalFormattingValue) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ConditionalFormattingValue[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ConditionalFormattingValue[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ConditionalFormattingValue[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ConditionalFormattingValue&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ConditionalFormattingValue) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ConditionalFormattingValue, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ConditionalFormattingValue, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ConditionalFormattingValue) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ConditionalFormattingValue, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ConditionalFormattingValue, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingValueCollectionDemo
    {
        public static void ConditionalFormattingValueCollectionExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägger till en tom villkorlig formatering
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Ställer in området för den villkorliga formateringen
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // Lägger till villkor
            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[conditionIndex];

            // Hämta ikonuppsättning
            IconSet iconSet = cond.IconSet;

            // Ange ikontyp
            iconSet.Type = IconSetType.Arrows3;

            // Hämta CFValueObjects-instansen
            ConditionalFormattingValueCollection cfvos = iconSet.Cfvos;

            // Lägg till ett nytt ConditionalFormattingValue i samlingen
            int cfvIndex = cfvos.Add(FormatConditionValueType.Number, "50");

            // Åtkomst till det nyss tillagda ConditionalFormattingValue
            ConditionalFormattingValue cfv = cfvos[cfvIndex];

            // Ändra egenskaperna för ConditionalFormattingValue
            cfv.Value = 75;
            cfv.Type = FormatConditionValueType.Percent;
            cfv.IsGTE = true;

            // Sätt cellvärden
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            // Sparar Excel-filen
            workbook.Save("ConditionalFormattingValueCollectionExample.xlsx");
            workbook.Save("ConditionalFormattingValueCollectionExample.pdf");
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [ConditionalFormattingValue](../conditionalformattingvalue/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


