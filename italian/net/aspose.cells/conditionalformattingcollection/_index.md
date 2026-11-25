---
title: "Classe ConditionalFormattingCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.ConditionalFormattingCollection. Incapsula una raccolta di oggetti FormatCondition"
type: docs
url: /it/net/aspose.cells/conditionalformattingcollection/
---
## ConditionalFormattingCollection class

Incapsula una raccolta di oggetti [`FormatCondition`](../formatcondition/).

```csharp
public class ConditionalFormattingCollection : CollectionBase<FormatConditionCollection>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/conditionalformattingcollection/item/) { get; } | Restituisce l'elemento FormatConditions all'indice specificato. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells/conditionalformattingcollection/add/)() | Aggiunge un FormatConditions alla raccolta. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(FormatConditionCollection) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(FormatConditionCollection, IComparer&lt;FormatConditionCollection&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, FormatConditionCollection, IComparer&lt;FormatConditionCollection&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(FormatConditionCollection) |  |
| [Copy](../../aspose.cells/conditionalformattingcollection/copy/)(ConditionalFormattingCollection) | Copia la formattazione condizionale. |
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
| [RemoveArea](../../aspose.cells/conditionalformattingcollection/removearea/)(int, int, int, int) | Rimuove tutta la formattazione condizionale nell'intervallo. |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Esempi

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

            // Aggiungi condizione.
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");

            // Imposta il colore di sfondo.
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            // Salvataggio del file Excel
            workbook.Save("ConditionalFormattingCollectionDemo.xlsx");
            workbook.Save("ConditionalFormattingCollectionDemo.pdf");
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [FormatConditionCollection](../formatconditioncollection/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


