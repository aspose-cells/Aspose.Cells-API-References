---
title: "Klass TableStyleElementCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Tables.TableStyleElementCollection-klass. Representerar alla element i tabellstilen"
type: docs
url: /sv/net/aspose.cells.tables/tablestyleelementcollection/
---
## TableStyleElementCollection class

Representerar alla element i tabellstilen.

```csharp
public class TableStyleElementCollection : CollectionBase<TableStyleElement>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.tables/tablestyleelementcollection/item/) { get; } | Hämtar ett element i tabellstilen efter index. (2 indexerare) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells.tables/tablestyleelementcollection/add/)(TableStyleElementType) | Lägger till ett element. |
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

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Skapa stilar för den första och sista kolumnen
            Style firstColumnStyle = workbook.CreateStyle();
            firstColumnStyle.Pattern = BackgroundType.Solid;
            firstColumnStyle.BackgroundColor = System.Drawing.Color.Red;

            Style lastColumnStyle = workbook.CreateStyle();
            lastColumnStyle.Font.IsBold = true;
            lastColumnStyle.Pattern = BackgroundType.Solid;
            lastColumnStyle.BackgroundColor = System.Drawing.Color.Red;

            // Definiera ett anpassat tabellstilsnamn
            string tableStyleName = "Custom1";

            // Få åtkomst till samlingen av tabellstilar
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

            // Lägg till en ny tabellstil i samlingen
            int index1 = tableStyles.AddTableStyle(tableStyleName);
            TableStyle tableStyle = tableStyles[index1];

            // Få åtkomst till samlingen av tabellstilelement
            TableStyleElementCollection elements = tableStyle.TableStyleElements;

            // Lägg till och konfigurera stil-elementet för den första kolumnen
            index1 = elements.Add(TableStyleElementType.FirstColumn);
            TableStyleElement element = elements[index1];
            element.SetElementStyle(firstColumnStyle);

            // Lägg till och konfigurera stil-elementet för den sista kolumnen
            index1 = elements.Add(TableStyleElementType.LastColumn);
            element = elements[index1];
            element.SetElementStyle(lastColumnStyle);

            // Fyll i kalkylbladet med exempeldata
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

            // Lägg till en tabell i kalkylbladet
            ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Tillämpa den anpassade tabellstilen på tabellen
            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.TableStyleName = tableStyleName;

            // Spara arbetsboken
            workbook.Save("TableStyleElementCollectionExample.xlsx");
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [TableStyleElement](../tablestyleelement/)
* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


