---
title: "Classe ConditionalFormattingValueCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.ConditionalFormattingValueCollection classe. Descrive una raccolta di CFValueObject. Utilizzare solo per set di icone"
type: docs
url: /it/net/aspose.cells/conditionalformattingvaluecollection/
---
## ConditionalFormattingValueCollection class

Descrive una raccolta di CFValueObject. Da usare solo per set di icone.

```csharp
public class ConditionalFormattingValueCollection : CollectionBase<ConditionalFormattingValue>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/conditionalformattingvaluecollection/item/) { get; } | Ottieni l'elemento CFValueObject all'indice specificato. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells/conditionalformattingvaluecollection/add/)(FormatConditionValueType, string) | Aggiunge l'oggetto [`ConditionalFormattingValue`](../conditionalformattingvalue/). |
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

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingValueCollectionDemo
    {
        public static void ConditionalFormattingValueCollectionExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiunge una formattazione condizionale vuota
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Imposta l'intervallo di formattazione condizionale
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // Aggiunge condizione
            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[conditionIndex];

            // Ottieni Icon Set
            IconSet iconSet = cond.IconSet;

            // Imposta tipo di icona
            iconSet.Type = IconSetType.Arrows3;

            // Ottieni l'istanza di CFValueObjects
            ConditionalFormattingValueCollection cfvos = iconSet.Cfvos;

            // Aggiungi un nuovo ConditionalFormattingValue alla raccolta
            int cfvIndex = cfvos.Add(FormatConditionValueType.Number, "50");

            // Accedi al ConditionalFormattingValue appena aggiunto
            ConditionalFormattingValue cfv = cfvos[cfvIndex];

            // Modifica le proprietà del ConditionalFormattingValue
            cfv.Value = 75;
            cfv.Type = FormatConditionValueType.Percent;
            cfv.IsGTE = true;

            // Inserisci valori delle celle
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            // Salvataggio del file Excel
            workbook.Save("ConditionalFormattingValueCollectionExample.xlsx");
            workbook.Save("ConditionalFormattingValueCollectionExample.pdf");
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [ConditionalFormattingValue](../conditionalformattingvalue/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


