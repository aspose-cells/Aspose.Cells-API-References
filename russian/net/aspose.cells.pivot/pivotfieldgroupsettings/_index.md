---
title: "Класс PivotFieldGroupSettings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Pivot.PivotFieldGroupSettings. Представляет настройку группы сводного поля"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfieldgroupsettings/
---
## PivotFieldGroupSettings class

Представляет настройку группы поля сводной таблицы.

```csharp
public class PivotFieldGroupSettings
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PivotFieldGroupSettings](pivotfieldgroupsettings/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| virtual [Type](../../aspose.cells.pivot/pivotfieldgroupsettings/type/) { get; } | Получает тип группы сводного поля. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldGroupSettingsDemo
    {
        public static void PivotFieldGroupSettingsExample()
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

            worksheet.Cells[0, 1].Value = "Amount";
            worksheet.Cells[1, 1].Value = 50;
            worksheet.Cells[2, 1].Value = 60;
            worksheet.Cells[3, 1].Value = 70;
            worksheet.Cells[4, 1].Value = 80;

            // Добавьте сводную таблицу на лист.
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавьте поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount

            // Получить доступ к полю строки
            PivotField rowField = pivotTable.RowFields[0];
            rowField.GroupBy(new CustomPiovtFieldGroupItem[] { new CustomPiovtFieldGroupItem("TestItemGroup", new int[] { 0, 1 }) }, true);

            // Получить доступ к настройкам группы поля строки
            PivotFieldGroupSettings groupSettings = rowField.GroupSettings;

            // Отобразить тип группы сводного поля
            Console.WriteLine("Group Type: " + groupSettings.Type);

            // Сохраните книгу
            workbook.Save("PivotFieldGroupSettingsExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


