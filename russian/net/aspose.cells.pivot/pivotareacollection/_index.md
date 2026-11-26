---
title: "Класс PivotAreaCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Pivot.PivotAreaCollection. Представляет список областей сводных таблиц"
type: docs
url: /ru/net/aspose.cells.pivot/pivotareacollection/
---
## PivotAreaCollection class

Представляет список областей сводной таблицы.

```csharp
public class PivotAreaCollection : CollectionBase<PivotArea>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.pivot/pivotareacollection/item/) { get; } | Получает объект [`PivotArea`](../pivotarea/); |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells.pivot/pivotareacollection/add/#add_1)(CellArea) | Добавляет область на основе представления сводной таблицы. |
| [Add](../../aspose.cells.pivot/pivotareacollection/add/#add)(PivotArea) | (**Устарело.**) Добавляет область сводной таблицы. |
| [AddPivotArea](../../aspose.cells.pivot/pivotareacollection/addpivotarea/)(PivotArea) | Добавляет область сводной таблицы в эту коллекцию. |
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
| [RemoveAt](../../aspose.cells.pivot/pivotareacollection/removeat/#removeat)(int) | Удалить одну настройку условного форматирования области сводной таблицы. (2 метода) |

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать примерные данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Electronics");
            worksheet.Cells["B2"].PutValue(1500);
            worksheet.Cells["A3"].PutValue("Clothing");
            worksheet.Cells["B3"].PutValue(800);
            worksheet.Cells["A4"].PutValue("Furniture");
            worksheet.Cells["B4"].PutValue(1200);

            // Добавить сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D3", "SalesPivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Создать ячейковые области для областей сводных таблиц
            CellArea dataArea = new CellArea { StartRow = 1, StartColumn = 1, EndRow = 4, EndColumn = 1 };
            CellArea headerArea = new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 1 };

            // Получить коллекцию областей сводных таблиц
            PivotAreaCollection pivotAreas = pivotTable.SelectArea(dataArea);

            // Добавить области сводных таблиц
            pivotAreas.Add(dataArea);
            pivotAreas.Add(headerArea);

            // Отобразить все области сводных таблиц
            Console.WriteLine("Pivot Areas Count: " + pivotAreas.Count);
            for (int i = 0; i < pivotAreas.Count; i++)
            {
                CellArea[] areas = pivotAreas[i].GetCellAreas();
                foreach (CellArea area in areas)
                {
                    Console.WriteLine($"Area {i}: ({area.StartRow},{area.StartColumn}) to ({area.EndRow},{area.EndColumn})");
                }
            }

            // Удалить область
            pivotAreas.RemoveAt(0);
            Console.WriteLine("\nAfter removal - Pivot Areas Count: " + pivotAreas.Count);

            // Сохраните книгу
            workbook.Save("PivotAreaCollectionDemo.xlsx");
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PivotArea](../pivotarea/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


