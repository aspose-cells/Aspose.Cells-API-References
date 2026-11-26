---
title: "Cells.GetLastDataRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получает индекс последней строки, содержащей данные в указанном столбце"
type: docs
url: /ru/net/aspose.cells/cells/getlastdatarow/
---
## Cells.GetLastDataRow method

Получает индекс последней строки ячейки, содержащей данные в указанном столбце.

```csharp
public int GetLastDataRow(int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| column | Int32 | Индекс столбца. |

### Возвращаемое значение

индекс последней строки.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetLastDataRowWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["A4"].PutValue("Data3");
            
            // Получить последнюю строку с данными в столбце A (индекс 0)
            int lastRow = worksheet.Cells.GetLastDataRow(0);
            
            // Вывести результат.
            Console.WriteLine("Last data row in column A: " + lastRow);
            
            // Вставить новую строку после последней строки с данными
            CellArea area = new CellArea();
            area.StartRow = lastRow + 1;
            area.EndRow = lastRow + 1;
            area.StartColumn = 0;
            area.EndColumn = 0;
            worksheet.Cells.InsertRange(area, 1, ShiftType.Down);
            
            // Добавить данные в новую строку
            worksheet.Cells[lastRow + 2, 0].PutValue("New Data");
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


