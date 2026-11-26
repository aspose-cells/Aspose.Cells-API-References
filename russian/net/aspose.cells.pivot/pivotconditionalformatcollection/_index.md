---
title: "Класс PivotConditionalFormatCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Pivot.PivotConditionalFormatCollection. Представляет все условные форматы сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotconditionalformatcollection/
---
## PivotConditionalFormatCollection class

Представляет все условные форматы сводной таблицы.

```csharp
public class PivotConditionalFormatCollection : CollectionBase<PivotConditionalFormat>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.pivot/pivotconditionalformatcollection/item/) { get; } | Получает объект FormatCondition сводной таблицы по указанному индексу. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells.pivot/pivotconditionalformatcollection/add/#add_1)() | Добавляет объект FormatCondition сводной таблицы в коллекцию. |
| [Add](../../aspose.cells.pivot/pivotconditionalformatcollection/add/#add)(int, int, PivotConditionFormatScopeType) | Применяет условное форматирование к диапазону, который должен находиться в области данных. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotConditionalFormat) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotConditionalFormat, IComparer&lt;PivotConditionalFormat&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, PivotConditionalFormat, IComparer&lt;PivotConditionalFormat&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(PivotConditionalFormat) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotConditionalFormat[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotConditionalFormat[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, PivotConditionalFormat[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;PivotConditionalFormat&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;PivotConditionalFormat&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;PivotConditionalFormat&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;PivotConditionalFormat&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;PivotConditionalFormat&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;PivotConditionalFormat&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;PivotConditionalFormat&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;PivotConditionalFormat&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;PivotConditionalFormat&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;PivotConditionalFormat&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotConditionalFormat) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotConditionalFormat, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotConditionalFormat, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotConditionalFormat) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotConditionalFormat, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotConditionalFormat, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotConditionalFormatCollectionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "A";
            cells["B2"].Value = "East";
            cells["C2"].Value = 100;
            
            cells["A3"].Value = "B";
            cells["B3"].Value = "West";
            cells["C3"].Value = 200;
            
            cells["A4"].Value = "C";
            cells["B4"].Value = "East";
            cells["C4"].Value = 300;
            
            cells["A5"].Value = "D";
            cells["B5"].Value = "West";
            cells["C5"].Value = 400;

            // Создать сводную таблицу
            int pivotIndex = sheet.PivotTables.Add("=A1:C5", "E3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            
            // Добавить поля в области сводной таблицы
            pivot.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivot.AddFieldToArea(PivotFieldType.Column, 1); // Region
            pivot.AddFieldToArea(PivotFieldType.Data, 2); // Sales

            // Обновить и вычислить сводную таблицу
            pivot.RefreshData();
            pivot.CalculateData();

            // Получить доступ к коллекции условных форматов
            PivotConditionalFormatCollection pfcc = pivot.ConditionalFormats;
            int formatIndex = pfcc.Add();
            PivotConditionalFormat pfc = pfcc[formatIndex];
            
            // Получить диапазон данных сводной таблицы
            CellArea dataBodyRange = pivot.DataBodyRange;
            pfc.FormatConditions.AddArea(dataBodyRange);

            // Добавить условное форматирование
            FormatConditionCollection fcc = pfc.FormatConditions;
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = fcc[conditionIndex];
            fc.Operator = OperatorType.Between;
            fc.Formula1 = "200";
            fc.Formula2 = "400";
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // Сохраните книгу
            workbook.Save("PivotConditionalFormatDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PivotConditionalFormat](../pivotconditionalformat/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


