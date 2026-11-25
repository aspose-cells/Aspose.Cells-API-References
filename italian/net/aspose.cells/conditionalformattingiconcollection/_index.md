---
title: "Classe ConditionalFormattingIconCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.ConditionalFormattingIconCollection. Rappresenta una raccolta di oggetti ConditionalFormattingIcon."
type: docs
url: /it/net/aspose.cells/conditionalformattingiconcollection/
---
## ConditionalFormattingIconCollection class

Rappresenta una raccolta di oggetti [`ConditionalFormattingIcon`](../conditionalformattingicon/).

```csharp
public class ConditionalFormattingIconCollection : CollectionBase<ConditionalFormattingIcon>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/conditionalformattingiconcollection/item/) { get; } | Recupera l'elemento ConditionalFormattingIcon all'indice specificato. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells/conditionalformattingiconcollection/add/#add)(ConditionalFormattingIcon) | (**Obsoleto.**) Aggiunge l'oggetto [`ConditionalFormattingIcon`](../conditionalformattingicon/). |
| [Add](../../aspose.cells/conditionalformattingiconcollection/add/#add_1)(IconSetType, int) | Aggiunge l'oggetto [`ConditionalFormattingIcon`](../conditionalformattingicon/). |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ConditionalFormattingIcon) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ConditionalFormattingIcon, IComparer&lt;ConditionalFormattingIcon&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ConditionalFormattingIcon, IComparer&lt;ConditionalFormattingIcon&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ConditionalFormattingIcon) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ConditionalFormattingIcon[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ConditionalFormattingIcon[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ConditionalFormattingIcon[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ConditionalFormattingIcon) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ConditionalFormattingIcon, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ConditionalFormattingIcon, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ConditionalFormattingIcon) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ConditionalFormattingIcon, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ConditionalFormattingIcon, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingIconCollectionDemo
    {
        public static void ConditionalFormattingIconCollectionExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ottieni la formattazione condizionale
            ConditionalFormattingCollection cformattings = sheet.ConditionalFormattings;

            // Aggiunge una formattazione condizionale vuota
            int index = cformattings.Add();

            // Ottieni la formattazione condizionale appena aggiunta
            FormatConditionCollection fcs = cformattings[index];

            // Imposta l'intervallo di formattazione condizionale.
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

            // Imposta la condizione
            int idx = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[idx];

            // Imposta il tipo della condizione
            cond.IconSet.Type = IconSetType.ArrowsGray3;

            // Aggiungi una condizione iconset personalizzata.
            ConditionalFormattingIcon cfIcon = cond.IconSet.CfIcons[0];
            cfIcon.Type = IconSetType.Arrows3;
            cfIcon.Index = 0;

            ConditionalFormattingIcon cfIcon1 = cond.IconSet.CfIcons[1];
            cfIcon1.Type = IconSetType.ArrowsGray3;
            cfIcon1.Index = 1;

            ConditionalFormattingIcon cfIcon2 = cond.IconSet.CfIcons[2];
            cfIcon2.Type = IconSetType.Boxes5;
            cfIcon2.Index = 2;

            // Salvataggio del file Excel
            workbook.Save("outConditionalFormattingIconCollectionDemoput.xlsx");
            workbook.Save("outConditionalFormattingIconCollectionDemoput.pdf");
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [ConditionalFormattingIcon](../conditionalformattingicon/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


