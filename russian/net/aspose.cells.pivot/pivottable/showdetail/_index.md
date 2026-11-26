---
title: "PivotTable.ShowDetail"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotTable. Показать детали одного элемента в области данных в новую таблицу"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/showdetail/
---
## PivotTable.ShowDetail method

Покажите детали одного элемента в области данных в новой таблице.

```csharp
public void ShowDetail(int rowOffset, int columnOffset, bool newSheet, int destRow, int destColumn)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowOffset | Int32 | Смещение к первой строке данных в области данных. |
| columnOffset | Int32 | Смещение к первому столбцу данных в области данных. |
| newSheet | Boolean | Показать детали на новом листе. |
| destRow | Int32 | Целевая строка. |
| destColumn | Int32 | Целевой столбец. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowDetailWithInt32Int32BooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Sport");
            worksheet.Cells["A2"].PutValue("Tennis");
            worksheet.Cells["A3"].PutValue("Basketball");
            worksheet.Cells["A4"].PutValue("Tennis");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(80);
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["B4"].PutValue(85);

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Sport");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Score");

            // Показать детали для конкретной ячейки
            pivotTable.ShowDetail(1, 0, true, 0, 0);

            // Сохраните книгу
            workbook.Save("PivotTableShowDetailExample.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


