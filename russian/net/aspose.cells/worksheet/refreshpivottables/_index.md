---
title: "Worksheet.RefreshPivotTables"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Обновляет все PivotTables в этом листе"
type: docs
url: /ru/net/aspose.cells/worksheet/refreshpivottables/
---
## RefreshPivotTables() {#refreshpivottables_1}

Обновляет все сводные таблицы в этом листе.

```csharp
public void RefreshPivotTables()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodRefreshPivotTablesDemo
    {
        public static void Run()
        {
            // Создайте книгу из исходного файла Excel, содержащего сводные таблицы
            Workbook workbook = new Workbook("example.xlsx");
            
            // Получите первый лист, содержащий сводные таблицы
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Обновите все сводные таблицы на листе
            worksheet.RefreshPivotTables();
            
            // Сохраните обновлённую книгу
            workbook.Save("RefreshedPivotTables.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RefreshPivotTables(PivotTableRefreshOption) {#refreshpivottables}

Обновляет все сводные таблицы в этом листе.

```csharp
public bool RefreshPivotTables(PivotTableRefreshOption option)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| опция | PivotTableRefreshOption | Опция для обновления источника данных сводной таблицы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class WorksheetMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;

            // Создайте сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            worksheet.RefreshPivotTables();

            int preCount = pivotTable.RowFields[0].PivotItems.Count;


            // Изменить исходные данные
            worksheet.Cells["A2"].Value = "test2";
            worksheet.Cells["A3"].Value = "test3";

            // Создать параметры обновления
            PivotTableRefreshOption options = new PivotTableRefreshOption
            {
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All // Fixed: Changed ReserveAll to All
            };
            worksheet.RefreshPivotTables(options);
            int nowCount = pivotTable.RowFields[0].PivotItems.Count;
            Console.WriteLine(nowCount > preCount);
                        

            // Сохранить результат
            workbook.Save("WorksheetMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTableRefreshOption](../../../aspose.cells.pivot/pivottablerefreshoption/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


