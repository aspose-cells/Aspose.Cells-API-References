---
title: "Class CheckBoxCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.CheckBoxCollection class. Rappresenta una collezione di oggetti CheckBox in un foglio di lavoro"
type: docs
url: /it/net/aspose.cells.drawing/checkboxcollection/
---
## CheckBoxCollection class

Rappresenta una collezione di oggetti [`CheckBox`](../checkbox/) in un foglio di lavoro.

```csharp
public class CheckBoxCollection : CollectionBase<CheckBox>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing/checkboxcollection/item/) { get; } | Ottiene l'elemento [`CheckBox`](../checkbox/) all'indice specificato. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells.drawing/checkboxcollection/add/)(int, int, int, int) | Aggiunge un checkBox alla collezione. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CheckBox) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CheckBox, IComparer&lt;CheckBox&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, CheckBox, IComparer&lt;CheckBox&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(CheckBox) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CheckBox[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CheckBox[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, CheckBox[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;CheckBox&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;CheckBox&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;CheckBox&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;CheckBox&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;CheckBox&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;CheckBox&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;CheckBox&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;CheckBox&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;CheckBox&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;CheckBox&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CheckBox) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CheckBox, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CheckBox, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CheckBox) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CheckBox, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CheckBox, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class CheckBoxCollectionDemo
    {
        public static void CheckBoxCollectionExample()
        {
            // Crea un nuovo Workbook.
            Workbook workbook = new Workbook();

            // Ottieni il primo foglio di lavoro nella cartella di lavoro.
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi un CheckBox al foglio di lavoro.
            int index = sheet.CheckBoxes.Add(15, 15, 20, 100);
            CheckBox checkBox = sheet.CheckBoxes[index];
            checkBox.Text = "Check Box 1";

            // Salva la cartella di lavoro.
            workbook.Save("CheckBoxCollectionExample.xlsx");
            workbook.Save("CheckBoxCollectionExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [CheckBox](../checkbox/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


