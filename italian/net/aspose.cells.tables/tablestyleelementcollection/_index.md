---
title: "Classe **TableStyleElementCollection**"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe **Aspose.Cells.Tables.TableStyleElementCollection**. Rappresenta tutti gli elementi dello stile della tabella"
type: docs
url: /it/net/aspose.cells.tables/tablestyleelementcollection/
---
## TableStyleElementCollection class

Rappresenta tutti gli elementi dello stile della tabella.

```csharp
public class TableStyleElementCollection : CollectionBase<TableStyleElement>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.tables/tablestyleelementcollection/item/) { get; } | Ottiene un elemento dello stile della tabella per indice. (2 indicizzatori) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells.tables/tablestyleelementcollection/add/)(TableStyleElementType) | Aggiunge un elemento. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(TableStyleElement) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(TableStyleElement, IComparer&lt;TableStyleElement&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, TableStyleElement, IComparer&lt;TableStyleElement&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(TableStyleElement) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(TableStyleElement[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(TableStyleElement[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, TableStyleElement[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;TableStyleElement&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;TableStyleElement&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;TableStyleElement&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;TableStyleElement&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;TableStyleElement&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;TableStyleElement&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;TableStyleElement&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;TableStyleElement&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;TableStyleElement&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;TableStyleElement&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TableStyleElement) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TableStyleElement, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TableStyleElement, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TableStyleElement) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TableStyleElement, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TableStyleElement, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleElementCollectionDemo
    {
        public static void TableStyleElementCollectionExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Crea stili per la prima e l'ultima colonna
            Style firstColumnStyle = workbook.CreateStyle();
            firstColumnStyle.Pattern = BackgroundType.Solid;
            firstColumnStyle.BackgroundColor = System.Drawing.Color.Red;

            Style lastColumnStyle = workbook.CreateStyle();
            lastColumnStyle.Font.IsBold = true;
            lastColumnStyle.Pattern = BackgroundType.Solid;
            lastColumnStyle.BackgroundColor = System.Drawing.Color.Red;

            // Definisci un nome di stile di tabella personalizzato
            string tableStyleName = "Custom1";

            // Accedi alla raccolta degli stili di tabella
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

            // Aggiungi un nuovo stile di tabella alla raccolta
            int index1 = tableStyles.AddTableStyle(tableStyleName);
            TableStyle tableStyle = tableStyles[index1];

            // Accedi alla raccolta degli elementi dello stile di tabella
            TableStyleElementCollection elements = tableStyle.TableStyleElements;

            // Aggiungi e configura l'elemento di stile della prima colonna
            index1 = elements.Add(TableStyleElementType.FirstColumn);
            TableStyleElement element = elements[index1];
            element.SetElementStyle(firstColumnStyle);

            // Aggiungi e configura l'elemento di stile dell'ultima colonna
            index1 = elements.Add(TableStyleElementType.LastColumn);
            element = elements[index1];
            element.SetElementStyle(lastColumnStyle);

            // Popola il foglio di lavoro con dati di esempio
            Cells cells = workbook.Worksheets[0].Cells;
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Aggiungi una tabella al foglio di lavoro
            ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Applica lo stile di tabella personalizzato alla tabella
            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.TableStyleName = tableStyleName;

            // Salva la cartella di lavoro
            workbook.Save("TableStyleElementCollectionExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [TableStyleElement](../tablestyleelement/)
* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


