---
title: "Класс FormatConditionCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.FormatConditionCollection. Представляет условное форматирование. FormatConditions может содержать до трёх условных форматов"
type: docs
url: /ru/net/aspose.cells/formatconditioncollection/
---
## FormatConditionCollection class

Представляет условное форматирование. Объект FormatConditions может содержать до трёх условных форматов.

```csharp
public class FormatConditionCollection
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.cells/formatconditioncollection/count/) { get; } | Получает количество условий. |
| [Item](../../aspose.cells/formatconditioncollection/item/) { get; } | Получает условие форматирования по индексу. |
| [RangeCount](../../aspose.cells/formatconditioncollection/rangecount/) { get; } | Получает количество условно отформатированных диапазонов. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells/formatconditioncollection/add/)(CellArea, FormatConditionType, OperatorType, string, string) | Добавляет условие форматирования и затронутый диапазон ячеек в FormatConditions. FormatConditions может содержать до трёх условных форматов. Ссылки на другие листы не допускаются в формулах условного форматирования. |
| [AddArea](../../aspose.cells/formatconditioncollection/addarea/)(CellArea) | Добавляет условно отформатированный диапазон ячеек. |
| [AddCondition](../../aspose.cells/formatconditioncollection/addcondition/#addcondition)(FormatConditionType) | Добавить условие форматирования. |
| [AddCondition](../../aspose.cells/formatconditioncollection/addcondition/#addcondition_1)(FormatConditionType, OperatorType, string, string) | Добавляет условие форматирования. |
| [GetCellArea](../../aspose.cells/formatconditioncollection/getcellarea/)(int) | Получает условно отформатированный диапазон ячеек по индексу. |
| [RemoveArea](../../aspose.cells/formatconditioncollection/removearea/#removearea_1)(int) | Удаляет условно отформатированный диапазон ячеек по индексу. |
| [RemoveArea](../../aspose.cells/formatconditioncollection/removearea/#removearea)(int, int, int, int) | Удалить условное форматирование в диапазоне. |
| [RemoveCondition](../../aspose.cells/formatconditioncollection/removecondition/)(int) | Удаляет условие форматирования по индексу. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionCollectionDemo
    {
        public static void FormatConditionCollectionExample()
        {
            // Создайте новую книгу
            Workbook workbook = new Workbook();

            // Получить первый лист
            Worksheet sheet = workbook.Worksheets[0];

            // Добавляет пустое условное форматирование
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Устанавливает диапазон условного форматирования
            CellArea ca = new CellArea { StartRow = 0, EndRow = 0, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);
            ca = new CellArea { StartRow = 1, EndRow = 1, StartColumn = 1, EndColumn = 1 };
            fcs.AddArea(ca);

            // Добавляет условия
            int conditionIndex1 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");

            // Устанавливает цвет фона
            FormatCondition fc1 = fcs[conditionIndex1];
            fc1.Style.BackgroundColor = System.Drawing.Color.Red;

            // Сохранение файла Excel
            workbook.Save("FormatConditionCollectionExample.xlsx");
            workbook.Save("FormatConditionCollectionExample.pdf");
            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


