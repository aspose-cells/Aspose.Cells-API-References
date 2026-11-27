---
title: "Klass PivotAreaCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotAreaCollection-klass. Representerar en lista med pivotområden"
type: docs
url: /sv/net/aspose.cells.pivot/pivotareacollection/
---
## PivotAreaCollection class

Representerar en lista över pivot‑område.

```csharp
public class PivotAreaCollection : CollectionBase<PivotArea>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.pivot/pivotareacollection/item/) { get; } | Hämtar ett [`PivotArea`](../pivotarea/) objekt; |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells.pivot/pivotareacollection/add/#add_1)(CellArea) | Lägger till ett område baserat på pivottabellvyn. |
| [Add](../../aspose.cells.pivot/pivotareacollection/add/#add)(PivotArea) | (**Obsolet.**) Lägger till pivotområde. |
| [AddPivotArea](../../aspose.cells.pivot/pivotareacollection/addpivotarea/)(PivotArea) | Lägger till pivotområde i denna samling. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotArea) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotArea, IComparer&lt;PivotArea&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, PivotArea, IComparer&lt;PivotArea&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(PivotArea) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotArea[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotArea[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, PivotArea[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;PivotArea&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;PivotArea&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;PivotArea&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;PivotArea&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;PivotArea&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;PivotArea&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;PivotArea&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;PivotArea&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;PivotArea&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;PivotArea&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotArea) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotArea, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotArea, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotArea) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotArea, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotArea, int, int) |  |
| [RemoveAt](../../aspose.cells.pivot/pivotareacollection/removeat/#removeat)(int) | Ta bort en pivots villkorligt formaterad områdesinställning. (2 metoder) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotAreaCollectionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata för pivottabell
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Electronics");
            worksheet.Cells["B2"].PutValue(1500);
            worksheet.Cells["A3"].PutValue("Clothing");
            worksheet.Cells["B3"].PutValue(800);
            worksheet.Cells["A4"].PutValue("Furniture");
            worksheet.Cells["B4"].PutValue(1200);

            // Lägg till en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D3", "SalesPivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Skapa cellområden för pivotområden
            CellArea dataArea = new CellArea { StartRow = 1, StartColumn = 1, EndRow = 4, EndColumn = 1 };
            CellArea headerArea = new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 1 };

            // Hämta pivotområdessamling
            PivotAreaCollection pivotAreas = pivotTable.SelectArea(dataArea);

            // Lägg till pivotområden
            pivotAreas.Add(dataArea);
            pivotAreas.Add(headerArea);

            // Visa alla pivottområden
            Console.WriteLine("Pivot Areas Count: " + pivotAreas.Count);
            for (int i = 0; i < pivotAreas.Count; i++)
            {
                CellArea[] areas = pivotAreas[i].GetCellAreas();
                foreach (CellArea area in areas)
                {
                    Console.WriteLine($"Area {i}: ({area.StartRow},{area.StartColumn}) to ({area.EndRow},{area.EndColumn})");
                }
            }

            // Ta bort ett område
            pivotAreas.RemoveAt(0);
            Console.WriteLine("\nAfter removal - Pivot Areas Count: " + pivotAreas.Count);

            // Spara arbetsboken
            workbook.Save("PivotAreaCollectionDemo.xlsx");
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PivotArea](../pivotarea/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


