---
title: "Klass ColumnCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ColumnCollection klass. Samling av Column‑objekt som representerar de enskilda kolumninställningarna i ett kalkylblad. Column‑objektet representerar endast inställningar såsom kolumnbredd, stilar osv. för hela kolumnen och har inget att göra med huruvida det finns icke‑tomma celldata i motsvarande kolumn. Och Count för denna samling representerar endast antalet Column‑objekt som har instansierats i samlingen och har inget att göra med huruvida det finns icke‑tomma celldata i kalkylbladet."
type: docs
url: /sv/net/aspose.cells/columncollection/
---
## ColumnCollection class

Samlings av [`Column`](../column/)‑objekt som representerar de enskilda kolumninställningarna i ett kalkylblad. Column‑objektet representerar endast inställningarna såsom kolumnbredd, stilar osv. för hela kolumnen och har inget att göra med huruvida det finns icke‑tomma celler (data) i motsvarande kolumn. Och "Count" för denna samling representerar endast antalet Column‑objekt som har instansierats i samlingen och har inget att göra med huruvida det finns icke‑tomma celler (data) i kalkylbladet.

```csharp
public class ColumnCollection : CollectionBase<Column>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/columncollection/item/) { get; } | Hämtar ett [`Column`](../column/)‑objekt efter kolumnindex. Column‑objektet för det angivna kolumnindexet kommer att instansieras om det inte redan finns. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
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
| [GetByIndex](../../aspose.cells/columncollection/getbyindex/)(int) | (**Föråldrad.**) Hämtar kolumnobjektet efter indexet. |
| [GetColumnByIndex](../../aspose.cells/columncollection/getcolumnbyindex/)(int) | Hämtar [`Column`](../column/)‑objektet efter positionen i listan. |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Column) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Column, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Column, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Column) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Column, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Column, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exempel

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
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();

            // Hämtning av referensen till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ny stil i arbetsboken
            Style style = workbook.CreateStyle();

            // Ställer in bakgrundsfärgen till blå
            style.ForegroundColor = Color.Blue;

            // Ställer in bakgrundsmönster
            style.Pattern = BackgroundType.Solid;

            // Ny stilflagga
            StyleFlag styleFlag = new StyleFlag();

            // Ställ in alla stilar
            styleFlag.All = true;

            // Ändra standardbredden för de första tio kolumnerna
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells.Columns[i].Width = 20;
            }

            // Hämta kolumnen med icke‑standardformatering
            ColumnCollection columns = worksheet.Cells.Columns;

            foreach (Column column in columns)
            {
                // Applicera stil på de första tio kolumnerna
                column.ApplyStyle(style, styleFlag);
            }

            // Sparar Excel-filen
            workbook.Save("ColumnCollectionExample.xlsx");
            workbook.Save("ColumnCollectionExample.pdf");
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Column](../column/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


