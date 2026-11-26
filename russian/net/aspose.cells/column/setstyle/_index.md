---
title: "Column.SetStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Column. Устанавливает стиль этого столбца"
type: docs
url: /ru/net/aspose.cells/column/setstyle/
---
## Column.SetStyle method

Задает стиль этого столбца.

```csharp
public void SetStyle(Style style)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| стиль | Стиль | стиль, который будет использоваться как стиль по умолчанию для ячеек в этом столбце. |

### Примечания

Этот метод только задаёт указанный стиль как стиль по умолчанию для этого столбца, не изменяя настройки стиля существующих ячеек в этом столбце. Чтобы одновременно обновить настройки стиля существующих ячеек до указанного стиля, пожалуйста, используйте [`ApplyStyle`](../applystyle/)

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnMethodSetStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить доступ к первой колонке
            Column column = worksheet.Cells.Columns[0];

            // Создать новый стиль из рабочей книги
            Style style = workbook.CreateStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = Color.LightBlue;
            style.Pattern = BackgroundType.Solid;

            try
            {
                // Применить пользовательский стиль ко всему столбцу
                column.SetStyle(style);
                
                Console.WriteLine($"Style applied successfully to column {column.Index}");
                Console.WriteLine($"Font: {style.Font.Name}, Size: {style.Font.Size}, Bold: {style.Font.IsBold}");
                Console.WriteLine($"Background: {style.ForegroundColor.Name}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStyle method: {ex.Message}");
            }

            // Сохранить изменённую книгу
            workbook.Save("ColumnMethodSetStyleDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


