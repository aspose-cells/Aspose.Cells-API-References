---
title: "Класс PivotDiscreteGroupSettings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Pivot.PivotDiscreteGroupSettings. Представляет дискретную группу поля сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotdiscretegroupsettings/
---
## PivotDiscreteGroupSettings class

Представляет дискретную группу поля сводной таблицы.

```csharp
public class PivotDiscreteGroupSettings : PivotFieldGroupSettings
```

## Свойства

| Имя | Описание |
| --- | --- |
| [DiscreteItems](../../aspose.cells.pivot/pivotdiscretegroupsettings/discreteitems/) { get; } | Получает дискретные элементы. |
| [Items](../../aspose.cells.pivot/pivotdiscretegroupsettings/items/) { get; } | (**Obsolete.**) Получает дискретные элементы. |
| override [Type](../../aspose.cells.pivot/pivotdiscretegroupsettings/type/) { get; } | Получает тип группы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotDiscreteGroupSettingsDemo
    {
        public static void PivotDiscreteGroupSettingsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавление некоторых образцовых данных
            worksheet.Cells[0, 0].PutValue("Item");
            worksheet.Cells[0, 1].PutValue("Quantity");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(15);
            worksheet.Cells[3, 0].PutValue("A");
            worksheet.Cells[3, 1].PutValue(10);
            worksheet.Cells[4, 0].PutValue("B");
            worksheet.Cells[4, 1].PutValue(15);

            // Добавьте сводную таблицу на лист.
            int pivotIndex = worksheet.PivotTables.Add("=A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Установить строки и поля данных
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Доступ к полю строки
            PivotField pivotField = pivotTable.RowFields[0];
            pivotField.GroupBy(new CustomPiovtFieldGroupItem[] { new CustomPiovtFieldGroupItem("TestItemGroup", new int[] { 0, 1}) }, true);

            // Создать экземпляр PivotDiscreteGroupSettings
            PivotDiscreteGroupSettings groupSettings = pivotField.GroupSettings as PivotDiscreteGroupSettings;

            // Установить тип группы в Discrete (Это свойство только для чтения)
            // Отобразить текущий тип группы
            Console.WriteLine("Group Type: " + groupSettings.Type);

            // Сохраните книгу
            workbook.Save("PivotDiscreteGroupSettingsExample.xlsx");

            return;
        }
    }
}
```

### См. также

* class [PivotFieldGroupSettings](../pivotfieldgroupsettings/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


