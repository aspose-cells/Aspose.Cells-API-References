---
title: "Класс PivotItemCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Pivot.PivotItemCollection. Представляет все объекты PivotItem в PivotField"
type: docs
url: /ru/net/aspose.cells.pivot/pivotitemcollection/
---
## PivotItemCollection class

Представляет все объекты [`PivotItem`](../pivotitem/) в PivotField.

```csharp
public class PivotItemCollection : CollectionBase<PivotItem>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.pivot/pivotitemcollection/item/) { get; } | Получает объект PivotItem по указанному индексу. (2 индексатора) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotItem) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotItem, IComparer&lt;PivotItem&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, PivotItem, IComparer&lt;PivotItem&gt;) |  |
| [ChangeitemsOrder](../../aspose.cells.pivot/pivotitemcollection/changeitemsorder/)(int, int) | (**Obsolete.**) Непосредственно изменяет порядок двух элементов. |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(PivotItem) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotItem[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotItem[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, PivotItem[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;PivotItem&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;PivotItem&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;PivotItem&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;PivotItem&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;PivotItem&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;PivotItem&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;PivotItem&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;PivotItem&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;PivotItem&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;PivotItem&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [HideAllDetail](../../aspose.cells.pivot/pivotitemcollection/hidealldetail/)(bool) | (**Obsolete.**) Устанавливает, скрывать ли все детали всех PivotItems в поле сводной таблицы. То есть сворачивает/разворачивает это поле. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotItem) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotItem, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotItem, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotItem) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotItem, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotItem, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
| [SwapItem](../../aspose.cells.pivot/pivotitemcollection/swapitem/)(int, int) | Непосредственно меняет местами два элемента. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemCollectionDemo
    {
        public static void PivotItemCollectionExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые данные в лист
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[4, 0].Value = "Date";

            worksheet.Cells[0, 1].Value = "Quantity";
            worksheet.Cells[1, 1].Value = 10;
            worksheet.Cells[2, 1].Value = 20;
            worksheet.Cells[3, 1].Value = 30;
            worksheet.Cells[4, 1].Value = 40;

            // Добавьте сводную таблицу на лист.
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Добавьте поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Quantity

            // Получить доступ к PivotField и его PivotItems
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            // Отобразить количество элементов pivot
            Console.WriteLine("Pivot Items Count: " + pivotItems.Count);

            // Перебрать элементы pivot и отобразить их имена
            foreach (PivotItem item in pivotItems)
            {
                Console.WriteLine("Pivot Item: " + item.Name);
            }

            // Изменить порядок элементов pivot
            pivotItems.ChangeitemsOrder(0, 2);

            // Сохраните книгу
            workbook.Save("PivotItemCollectionExample.xlsx");

            return;
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PivotItem](../pivotitem/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


