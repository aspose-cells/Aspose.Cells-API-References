---
title: "PivotTable.GetCellByDisplayName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotTable. Получает объект Cell по отображаемому имени PivotField"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/getcellbydisplayname/
---
## PivotTable.GetCellByDisplayName method

Получает объект [`Cell`](../../../aspose.cells/cell/) по отображаемому имени PivotField.

```csharp
public Cell GetCellByDisplayName(string displayName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| displayName | String | Отображаемое имя DisplayName PivotField |

### Возвращаемое значение

Объект Cell

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetCellByDisplayNameWithStringDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Создать сводную таблицу
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Добавить поле строки и поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Обновить и вычислить сводную таблицу
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Получить отображаемое имя поля данных
            string displayName = pivotTable.DataFields[0].DisplayName;

            // Использовать метод GetCellByDisplayName
            Cell cell = pivotTable.GetCellByDisplayName(displayName);

            // Вывести результаты
            Console.WriteLine("Display Name: " + displayName);
            Console.WriteLine("Cell Name: " + (cell != null ? cell.Name : "null"));
            Console.WriteLine("Cell Value: " + (cell != null ? cell.Value.ToString() : "null"));

            // Сохраните книгу
            workbook.Save("PivotTable_GetCellByDisplayName_Output.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../../../aspose.cells/cell/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


