---
title: "Klasse TableStyleElementCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Tables.TableStyleElementCollection Klasse. Stellt alle Elemente des Tabellenstils dar"
type: docs
url: /de/net/aspose.cells.tables/tablestyleelementcollection/
---
## TableStyleElementCollection class

Stellt alle Elemente des Tabellenvorlagestils dar.

```csharp
public class TableStyleElementCollection : CollectionBase<TableStyleElement>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.tables/tablestyleelementcollection/item/) { get; } | Liefert ein Element des Tabellenstils nach dem Index. (2 Indexer) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells.tables/tablestyleelementcollection/add/)(TableStyleElementType) | Fügt ein Element hinzu. |
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

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Erstelle Stile für die erste und letzte Spalte
            Style firstColumnStyle = workbook.CreateStyle();
            firstColumnStyle.Pattern = BackgroundType.Solid;
            firstColumnStyle.BackgroundColor = System.Drawing.Color.Red;

            Style lastColumnStyle = workbook.CreateStyle();
            lastColumnStyle.Font.IsBold = true;
            lastColumnStyle.Pattern = BackgroundType.Solid;
            lastColumnStyle.BackgroundColor = System.Drawing.Color.Red;

            // Definiere einen benutzerdefinierten Tabellestilnamen
            string tableStyleName = "Custom1";

            // Greife auf die Sammlung der Tabellestile zu
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

            // Fügen Sie der Sammlung einen neuen Tabellestil hinzu
            int index1 = tableStyles.AddTableStyle(tableStyleName);
            TableStyle tableStyle = tableStyles[index1];

            // Greifen Sie auf die Sammlung der Tabellestil-Elemente zu
            TableStyleElementCollection elements = tableStyle.TableStyleElements;

            // Fügen Sie das Stil-Element der ersten Spalte hinzu und konfigurieren Sie es
            index1 = elements.Add(TableStyleElementType.FirstColumn);
            TableStyleElement element = elements[index1];
            element.SetElementStyle(firstColumnStyle);

            // Fügen Sie das Stil-Element der letzten Spalte hinzu und konfigurieren Sie es
            index1 = elements.Add(TableStyleElementType.LastColumn);
            element = elements[index1];
            element.SetElementStyle(lastColumnStyle);

            // Arbeitsblatt mit Beispieldaten füllen
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

            // Fügen Sie dem Arbeitsblatt eine Tabelle hinzu
            ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Wenden Sie den benutzerdefinierten Tabellestil auf die Tabelle an
            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.TableStyleName = tableStyleName;

            // Speichere die Arbeitsmappe
            workbook.Save("TableStyleElementCollectionExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [TableStyleElement](../tablestyleelement/)
* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


