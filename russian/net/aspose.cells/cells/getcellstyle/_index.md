---
title: "Cells.GetCellStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получить стиль заданной ячейки"
type: docs
url: /ru/net/aspose.cells/cells/getcellstyle/
---
## Cells.GetCellStyle method

Получить стиль заданной ячейки.

```csharp
public Style GetCellStyle(int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | индекс строки |
| column | Int32 | column |

### Возвращаемое значение

стиль заданной ячейки.

### Примечания

Возвращаемый стиль — это только тот, который установлен для ячейки или унаследован из строки/столбца ячейки, он не включает свойства, применённые другими настройками, такими как условное форматирование.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsMethodGetCellStyleWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получите доступ к ячейке B5 (строка 4, столбец 1) и задайте начальный стиль
            Cell cell = worksheet.Cells["B5"];
            cell.PutValue("Styled Cell");
            
            // Создайте и примените начальный стиль ячейки
            Style initialStyle = workbook.CreateStyle();
            initialStyle.Font.IsBold = true;  // Changed from Bold to IsBold
            initialStyle.BackgroundColor = Color.LightYellow;
            cell.SetStyle(initialStyle);

            try
            {
                // Вызовите GetCellStyle с параметрами Int32 (строка 4, столбец 1)
                Style cellStyle = worksheet.Cells.GetCellStyle(4, 1);

                // Отобразите полученные свойства стиля
                Console.WriteLine($"Retrieved style - Bold: {cellStyle.Font.IsBold}, Background: {cellStyle.BackgroundColor}");  // Changed from Bold to IsBold

                // Измените полученный стиль
                cellStyle.Font.IsItalic = true;  // Changed from Italic to IsItalic
                cellStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;

                // Примените изменённый стиль обратно к ячейке
                cell.SetStyle(cellStyle);

                Console.WriteLine("GetCellStyle executed successfully. Modified border and font style.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellStyle: {ex.Message}");
            }

            // Сохранить изменённую книгу
            workbook.Save("CellsGetCellStyleWithInt32Demo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


