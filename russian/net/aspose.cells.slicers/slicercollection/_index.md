---
title: "Класс SlicerCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Slicers.SlicerCollection. Указывает коллекцию всех объектов Slicer на указанном листе"
type: docs
url: /ru/net/aspose.cells.slicers/slicercollection/
---
## SlicerCollection class

Указывает коллекцию всех объектов Slicer на указанном листе.

```csharp
public class SlicerCollection : CollectionBase<Slicer>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.slicers/slicercollection/item/) { get; } | Получает Slicer по индексу. (2 индексатора) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells.slicers/slicercollection/add/#add_8)(ListObject, int, string) | Добавьте новый Slicer, используя ListObjet в качестве источника данных |
| [Add](../../aspose.cells.slicers/slicercollection/add/#add_7)(ListObject, ListColumn, string) | Добавьте новый Slicer, используя ListObjet в качестве источника данных |
| [Add](../../aspose.cells.slicers/slicercollection/add/#add_4)(PivotTable, string, int) | Добавить новый Slicer, используя PivotTable в качестве источника данных |
| [Add](../../aspose.cells.slicers/slicercollection/add/#add_3)(PivotTable, string, PivotField) | Добавить новый Slicer, используя PivotTable в качестве источника данных |
| [Add](../../aspose.cells.slicers/slicercollection/add/#add_5)(PivotTable, string, string) | Добавить новый Slicer, используя PivotTable в качестве источника данных |
| [Add](../../aspose.cells.slicers/slicercollection/add/#add_6)(ListObject, ListColumn, int, int) | Добавьте новый Slicer, используя ListObjet в качестве источника данных |
| [Add](../../aspose.cells.slicers/slicercollection/add/#add_1)(PivotTable, int, int, int) | Добавить новый Slicer, используя PivotTable в качестве источника данных |
| [Add](../../aspose.cells.slicers/slicercollection/add/#add)(PivotTable, int, int, PivotField) | Добавить новый Slicer, используя PivotTable в качестве источника данных |
| [Add](../../aspose.cells.slicers/slicercollection/add/#add_2)(PivotTable, int, int, string) | Добавить новый Slicer, используя PivotTable в качестве источника данных |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Slicer) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Slicer, IComparer&lt;Slicer&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Slicer, IComparer&lt;Slicer&gt;) |  |
| [Clear](../../aspose.cells.slicers/slicercollection/clear/#clear)() | Очистить все Slicers. (2 метода) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Slicer) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Slicer[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Slicer[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Slicer[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Slicer&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Slicer&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Slicer&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Slicer&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Slicer&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Slicer&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Slicer&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Slicer&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Slicer&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Slicer&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Slicer) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Slicer, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Slicer, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Slicer) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Slicer, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Slicer, int, int) |  |
| [Remove](../../aspose.cells.slicers/slicercollection/remove/)(Slicer) | Удалить указанный Slicer |
| [RemoveAt](../../aspose.cells.slicers/slicercollection/removeat/#removeat)(int) | Удаляет Slicer по указанному индексу (2 метода) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using Aspose.Cells.Slicers;
    using Aspose.Cells.Tables;
    using System;

    public class SlicerCollectionDemo
    {
        public static void SlicerCollectionExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Заполнить лист образцовыми данными
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";

            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;

            // Добавить сводную таблицу
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            pivot.RefreshData();
            pivot.CalculateData();

            // Получить коллекцию slicer
            SlicerCollection slicers = sheet.Slicers;

            // Добавить slicer на лист
            int slicerIndex = slicers.Add(pivot, "E2", "fruit");

            // Получить доступ к slicer
            Slicer slicer = slicers[slicerIndex];

            // Установить некоторые свойства slicer
            slicer.Caption = "Fruit Slicer";
            slicer.StyleType = SlicerStyleType.SlicerStyleLight1;

            // Сохраните книгу
            workbook.Save("SlicerCollectionExample.xlsx");
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [Slicer](../slicer/)
* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


