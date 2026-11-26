---
title: "Cells.GetCellDisplayStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получает стиль отображения указанной ячейки"
type: docs
url: /ru/net/aspose.cells/cells/getcelldisplaystyle/
---
## GetCellDisplayStyle(int, int) {#getcelldisplaystyle}

Получить стиль отображения заданной ячейки.

```csharp
public Style GetCellDisplayStyle(int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | индекс строки указанной ячейки |
| column | Int32 | столбец указанной ячейки |

### Возвращаемое значение

стиль отображения указанной ячейки.

### Примечания

То же самое с [`GetDisplayStyle`](../../cell/getdisplaystyle/), и то же самое при использовании SideBorders для `GetCellDisplayStyle`.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetCellDisplayStyleWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Подготовьте стиль ячейки для демонстрации
            Cell cell = cells[0, 0];
            cell.PutValue("Style Demo");
            
            // Создайте пользовательский стиль
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            
            // Примените стиль к ячейке
            cell.SetStyle(style);

            try
            {
                // Вызовите GetCellDisplayStyle с строкой 0 и столбцом 0
                Style displayStyle = cells.GetCellDisplayStyle(0, 0);

                // Свойства стиля отображения
                Console.WriteLine($"Bold: {displayStyle.Font.IsBold}");
                Console.WriteLine($"Background Color: {displayStyle.ForegroundColor}");

                // Примените стиль отображения к другой ячейке для визуальной проверки
                cells[2, 2].SetStyle(displayStyle);
                cells[2, 2].PutValue("Style Copied");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellDisplayStyle method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("CellsMethodGetCellDisplayStyleWithInt32Int32Demo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCellDisplayStyle(int, int, BorderType) {#getcelldisplaystyle_1}

Получить стиль отображения заданной ячейки.

```csharp
public Style GetCellDisplayStyle(int row, int column, BorderType adjacentBorders)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | индекс строки указанной ячейки |
| column | Int32 | столбец указанной ячейки |
| adjacentBorders | BorderType | Указывает, какие границы необходимо проверить и скорректировать в соответствии с границами соседних ячеек. Пожалуйста, см. описание того же параметра в [`GetDisplayStyle`](../../cell/getdisplaystyle/). |

### Возвращаемое значение

стиль отображения указанной ячейки.

### Примечания

Если ячейка также затронута другими настройками, такими как условное форматирование, объекты списка и т.д., то стиль отображения может отличаться от [`GetCellStyle`](../getcellstyle/). И поскольку эти настройки также могут применяться к пустым (несуществующим) ячейкам, использование этого метода может избежать создания таких пустых ячеек, поэтому производительность будет лучше, чем получение экземпляра Cell из Cells и последующий вызов [`GetDisplayStyle`](../../cell/getdisplaystyle/).

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetCellDisplayStyleWithInt32Int32BorderTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить доступ к ячейке A1 и установить стиль границы
            Cell cell = worksheet.Cells["A1"];
            Style style = cell.GetStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;
            cell.SetStyle(style);

            try
            {
                // Вызвать GetCellDisplayStyle с конкретными параметрами (0,0 для A1, тип TopBorder)
                Style displayStyle = worksheet.Cells.GetCellDisplayStyle(0, 0, BorderType.TopBorder);

                // Проверить, соответствует ли полученный стиль нашему цвету границы
                if (displayStyle.Borders[BorderType.TopBorder].Color == System.Drawing.Color.Red)
                {
                    Console.WriteLine("Top border display style retrieved successfully - Color: Red");
                }

                // Продемонстрировать применение стиля, изменив другую ячейку
                Cell targetCell = worksheet.Cells["B1"];
                targetCell.SetStyle(displayStyle);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellDisplayStyle method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("GetCellDisplayStyleWithBorderTypeDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../style/)
* enum [BorderType](../../bordertype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


