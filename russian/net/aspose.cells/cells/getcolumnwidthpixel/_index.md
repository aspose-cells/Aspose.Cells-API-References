---
title: "Cells.GetColumnWidthPixel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получает ширину указанного столбца в обычном виде в пикселях"
type: docs
url: /ru/net/aspose.cells/cells/getcolumnwidthpixel/
---
## GetColumnWidthPixel(int) {#getcolumnwidthpixel}

Получает ширину указанного столбца в обычном виде, в единицах пикселей.

```csharp
public int GetColumnWidthPixel(int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| column | Int32 | Индекс столбца |

### Возвращаемое значение

Ширина столбца в обычном виде.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetColumnWidthPixelWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить ширину столбца в символах (будет преобразовано в пиксели)
            worksheet.Cells.SetColumnWidth(1, 25);
            
            // Получить ширину столбца в пикселях
            int widthInPixels = worksheet.Cells.GetColumnWidthPixel(1);
            
            // Вывести результат.
            Console.WriteLine("Column width in pixels: " + widthInPixels);
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetColumnWidthPixel(int, bool) {#getcolumnwidthpixel_1}

Получает ширину указанного столбца в обычном виде, в единицах пикселей.

```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int GetColumnWidthPixel(int column, bool original)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| column | Int32 | Индекс столбца |
| исходный | Boolean | Указывает, возвращать ли исходную ширину, даже если столбец скрыт |

### Возвращаемое значение

Ширина столбца в обычном виде.

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод Cells.GetColumnWidth(int ,bool , CellsUnitType ). Этот метод будет удалён через 12 месяцев, начиная с апреля 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetColumnWidthPixelWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить стандартную ширину столбца в 80 пикселей
            worksheet.Cells.StandardWidthPixels = 80;

            // Установить конкретную ширину столбца для столбца 2 (третьего столбца) в 120 пикселей
            worksheet.Cells.SetColumnWidthPixel(2, 120);

            try
            {
                // Получить текущую ширину с пользовательскими изменениями (original: false)
                int currentWidth = worksheet.Cells.GetColumnWidthPixel(2, false);
                Console.WriteLine($"Column 2 current width: {currentWidth} pixels");

                // Получить исходную ширину без изменений (original: true)
                int originalWidth = worksheet.Cells.GetColumnWidthPixel(2, true);
                Console.WriteLine($"Column 2 original width: {originalWidth} pixels");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetColumnWidthPixel: {ex.Message}");
            }

            // Сохранить книгу, чтобы продемонстрировать сохранность ширины столбцов
            workbook.Save("ColumnWidthDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


