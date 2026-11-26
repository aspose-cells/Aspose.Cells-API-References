---
title: "Класс PivotItem"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Pivot.PivotItem класс. Представляет элемент в отчете PivotField."
type: docs
url: /ru/net/aspose.cells.pivot/pivotitem/
---
## PivotItem class

Представляет элемент в отчете PivotField.

```csharp
public class PivotItem
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Index](../../aspose.cells.pivot/pivotitem/index/) { get; set; } | (**Obsolete.**) Получает индекс элемента сводки в поле кэша. |
| [IsCalculatedItem](../../aspose.cells.pivot/pivotitem/iscalculateditem/) { get; } | Указывает, является ли этот элемент сводки вычисляемым элементом формулы. |
| [IsDetailHidden](../../aspose.cells.pivot/pivotitem/isdetailhidden/) { get; set; } | Получает и задает, скрыты ли детали этого элемента сводки. |
| [IsFormula](../../aspose.cells.pivot/pivotitem/isformula/) { get; set; } | (**Obsolete.**) Указывает, является ли этот элемент сводки вычисляемым элементом формулы. |
| [IsHidden](../../aspose.cells.pivot/pivotitem/ishidden/) { get; set; } | Получает и задает, скрыт ли элемент сводки. |
| [IsHideDetail](../../aspose.cells.pivot/pivotitem/ishidedetail/) { get; set; } | (**Obsolete.**) Получает и задает, скрывает ли элемент сводки детали. |
| [IsMissing](../../aspose.cells.pivot/pivotitem/ismissing/) { get; } | Указывает, был ли элемент удалён из источника данных. |
| [Name](../../aspose.cells.pivot/pivotitem/name/) { get; set; } | Получает имя элемента сводки. |
| [Position](../../aspose.cells.pivot/pivotitem/position/) { get; set; } | Указывает индекс этого элемента среди всех PivotItems поля. |
| [PositionInSameParentNode](../../aspose.cells.pivot/pivotitem/positioninsameparentnode/) { get; set; } | (**Obsolete.**) Указывает позиционный индекс в PivotItems под тем же родительским узлом. |
| [Value](../../aspose.cells.pivot/pivotitem/value/) { get; } | Получает значение элемента сводки |

## Методы

| Имя | Описание |
| --- | --- |
| [GetDateTimeValue](../../aspose.cells.pivot/pivotitem/getdatetimevalue/)() | Получает значение даты и времени элемента сводки. Если значение равно null, будет возвращено DateTime.MinValue |
| [GetDoubleValue](../../aspose.cells.pivot/pivotitem/getdoublevalue/)() | Получает двойное значение элемента сводки. Если значение равно null или не является числом, будет возвращено 0 |
| [GetFormula](../../aspose.cells.pivot/pivotitem/getformula/)() | Получает формулу этого вычисляемого элемента. Работает только когда элемент является вычисляемым. |
| [GetStringValue](../../aspose.cells.pivot/pivotitem/getstringvalue/)() | Получает строковое значение элемента сводки. Если значение равно null, будет возвращена пустая строка "" |
| [Move](../../aspose.cells.pivot/pivotitem/move/#move)(int) | Перемещает элемент вверх или вниз в поле сводки |
| [Move](../../aspose.cells.pivot/pivotitem/move/#move_1)(int, bool) | (**Obsolete.**) Перемещает элемент вверх или вниз |

## Поля

| Имя | Описание |
| --- | --- |
| const [AllPageItemsIndex](../../aspose.cells.pivot/pivotitem/allpageitemsindex/) | Индекс-сторож выбора всех элементов страницы (0x7FFD, недействительный индекс) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemDemo
    {
        public static void PivotItemExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые данные в лист
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Vegetable");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            // Добавьте сводную таблицу на лист.
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавьте поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Доступ к элементам сводки
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            int pivotItemCount = pivotItems.Count;
            Console.WriteLine("Number of Pivot Items: " + pivotItemCount);
            for(int i = 0; i < pivotItemCount; i++)
            {
                PivotItem pivotItem = pivotItems[i];
                // Вывести имя элемента сводки
                Console.WriteLine("Pivot Item Name: " + pivotItem.Name);

                // Установить свойства
                pivotItem.IsHidden = false;
                pivotItem.Position = 1;
                pivotItem.IsHideDetail = false;

                // Вывести значение элемента сводки
                Console.WriteLine("Pivot Item Value: " + pivotItem.Value);

                // Использовать методы
                string stringValue = pivotItem.GetStringValue();
                double doubleValue = pivotItem.GetDoubleValue();
                DateTime dateTimeValue = pivotItem.GetDateTimeValue();

                Console.WriteLine("String Value: " + stringValue);
                Console.WriteLine("Double Value: " + doubleValue);
                Console.WriteLine("DateTime Value: " + dateTimeValue);
            }

            // Сохраните книгу
            workbook.Save("PivotItemExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


