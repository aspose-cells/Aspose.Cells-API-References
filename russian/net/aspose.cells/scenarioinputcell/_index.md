---
title: "Класс ScenarioInputCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.ScenarioInputCell. Представляет входную ячейку для сценария"
type: docs
url: /ru/net/aspose.cells/scenarioinputcell/
---
## ScenarioInputCell class

Представляет входную ячейку для сценария.

```csharp
public class ScenarioInputCell
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Column](../../aspose.cells/scenarioinputcell/column/) { get; } | Получает и задает индекс столбца входной ячейки. |
| [IsDeleted](../../aspose.cells/scenarioinputcell/isdeleted/) { get; set; } | Указывает, удалена ли входная ячейка. |
| [Name](../../aspose.cells/scenarioinputcell/name/) { get; } | Получает и задает адрес входной ячейки. |
| [Row](../../aspose.cells/scenarioinputcell/row/) { get; } | Получает и задает индекс строки входной ячейки. |
| [Value](../../aspose.cells/scenarioinputcell/value/) { get; set; } | Получает и задает значение входной ячейки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ScenarioInputCellDemo
    {
        public static void ScenarioInputCellExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить сценарий в рабочий лист
            int scenarioIndex = worksheet.Scenarios.Add("Scenario 1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Добавить входные ячейки в сценарий
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(0, 0, "100"); // Adding cell A1 with value 100
            inputCells.Add(1, 1, "200"); // Adding cell B2 with value 200

            // Доступ к входным ячейкам
            ScenarioInputCell inputCell1 = inputCells[0];
            ScenarioInputCell inputCell2 = inputCells[1];

            // Отображение свойств входных ячеек
            Console.WriteLine($"Input Cell 1: Row = {inputCell1.Row}, Column = {inputCell1.Column}, Value = {inputCell1.Value}, IsDeleted = {inputCell1.IsDeleted}");
            Console.WriteLine($"Input Cell 2: Row = {inputCell2.Row}, Column = {inputCell2.Column}, Value = {inputCell2.Value}, IsDeleted = {inputCell2.IsDeleted}");

            // Изменить значение первой входной ячейки
            inputCell1.Value = "150";

            // Сохраните книгу
            workbook.Save("ScenarioInputCellExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


