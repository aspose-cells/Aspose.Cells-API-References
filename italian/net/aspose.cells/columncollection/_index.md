---
title: "Classe ColumnCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.ColumnCollection class. Collezione degli oggetti Column che rappresentano le singole impostazioni di colonna in un foglio di lavoro. L'oggetto Column rappresenta solo le impostazioni come larghezza della colonna, stili, ecc., per l'intera colonna e non ha nulla a che fare con il fatto che vi siano o meno celle non vuote nella colonna corrispondente. Inoltre, il Count di questa collezione rappresenta solo il numero di oggetti Column che sono stati istanziati in questa collezione, senza alcuna relazione con la presenza di celle non vuote nel foglio di lavoro."
type: docs
url: /it/net/aspose.cells/columncollection/
---
## ColumnCollection class

Collezione degli oggetti [`Column`](../column/) che rappresentano le singole impostazioni di colonna in un foglio di lavoro. L'oggetto Column rappresenta solo le impostazioni come larghezza della colonna, stili, ecc., per l'intera colonna e non ha nulla a che fare con il fatto che vi siano o meno celle non vuote (dati) nella colonna corrispondente. Inoltre, il "Count" di questa collezione rappresenta solo il numero di oggetti Column che sono stati istanziati in questa collezione, senza alcuna relazione con la presenza di celle non vuote (dati) nel foglio di lavoro.

```csharp
public class ColumnCollection : CollectionBase<Column>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/columncollection/item/) { get; } | Ottiene un oggetto [`Column`](../column/) tramite l'indice di colonna. L'oggetto Column dell'indice di colonna specificato verrà istanziato se non esiste già. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Column) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Column, IComparer&lt;Column&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Column, IComparer&lt;Column&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Column) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Column[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Column[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Column[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Column&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Column&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Column&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Column&gt;) |  |
| [GetByIndex](../../aspose.cells/columncollection/getbyindex/)(int) | (**Obsoleto.**) Ottiene l'oggetto colonna tramite l'indice. |
| [GetColumnByIndex](../../aspose.cells/columncollection/getcolumnbyindex/)(int) | Ottiene l'oggetto [`Column`](../column/) in base alla posizione nella lista. |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Column) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Column, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Column, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Column) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Column, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Column, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnCollectionDemo
    {
        public static void ColumnCollectionExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();

            // Ottenere il riferimento del primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un nuovo Stile al Workbook
            Style style = workbook.CreateStyle();

            // Impostazione del colore di sfondo su Blu
            style.ForegroundColor = Color.Blue;

            // Impostazione del modello di sfondo
            style.Pattern = BackgroundType.Solid;

            // Nuovo flag di stile
            StyleFlag styleFlag = new StyleFlag();

            // Imposta tutti gli stili
            styleFlag.All = true;

            // Modifica la larghezza predefinita delle prime dieci colonne
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells.Columns[i].Width = 20;
            }

            // Ottieni la Column con formattazione non predefinita
            ColumnCollection columns = worksheet.Cells.Columns;

            foreach (Column column in columns)
            {
                // Applica lo Stile alle prime dieci Column
                column.ApplyStyle(style, styleFlag);
            }

            // Salvataggio del file Excel
            workbook.Save("ColumnCollectionExample.xlsx");
            workbook.Save("ColumnCollectionExample.pdf");
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Column](../column/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


