---
title: "PivotFieldGroupSettings.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotFieldGroupSettings. Возвращает тип группы поля сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfieldgroupsettings/type/
---
## PivotFieldGroupSettings.Type property

Получает тип группы сводного поля.

```csharp
public virtual PivotFieldGroupType Type { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldGroupSettingsPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].Value = "Date";
            worksheet.Cells["A2"].Value = new DateTime(2023, 1, 1);
            worksheet.Cells["A3"].Value = new DateTime(2023, 1, 2);
            worksheet.Cells["A4"].Value = new DateTime(2023, 1, 3);

            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            try
            {
                // Добавьте сводную таблицу на лист.
                int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B4", "D3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Добавьте поля в сводную таблицу
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Date
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

                // Получить доступ к полю строки и сгруппировать по дате
                PivotField rowField = pivotTable.RowFields[0];
                rowField.GroupBy(new CustomPiovtFieldGroupItem[] { new CustomPiovtFieldGroupItem("DateGroup", new int[] { 0, 1 }) }, true);

                // Получить доступ к настройкам группы поля строки
                PivotFieldGroupSettings groupSettings = rowField.GroupSettings;

                // Отобразить текущее значение свойства Type (только для чтения)
                Console.WriteLine("Pivot Field Group Type: " + groupSettings.Type);

                // Сохраните книгу
                workbook.Save("PivotFieldGroupSettingsTypeDemo.xlsx");
                Console.WriteLine("Type property has been demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [PivotFieldGroupType](../../pivotfieldgrouptype/)
* class [PivotFieldGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


