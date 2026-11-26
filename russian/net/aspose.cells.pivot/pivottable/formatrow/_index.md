---
title: "PivotTable.FormatRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotTable. Форматировать данные строки в области сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/formatrow/
---
## PivotTable.FormatRow method

Форматирует данные строк в области сводной таблицы

```csharp
public void FormatRow(int row, Style style)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки объекта Row |
| стиль | Стиль | Стиль, который используется для форматирования |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodFormatRowWithInt32StyleDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            
            // Пример данных для сводной таблицы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(40);

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Создать стиль для форматирования
            Style style = wb.CreateStyle();
            style.Custom = "0.00%";
            style.Font.Name = "Calibri";
            style.Font.Size = 11;
            
            // Найти и отформатировать строки
            Cell cell = worksheet.Cells.Find("A", null);
            if (cell != null)
            {
                pivotTable.FormatRow(cell.Row, style);
            }
            
            cell = worksheet.Cells.Find("B", null);
            if (cell != null)
            {
                pivotTable.FormatRow(cell.Row, style);
            }
            
            // Сохраните книгу
            wb.Save("PivotTableFormatRowDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


