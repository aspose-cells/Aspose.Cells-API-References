---
title: "Column.Style"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Column. Возвращает стиль этой колонки"
type: docs
url: /ru/net/aspose.cells/column/style/
---
## Column.Style property

Получает стиль этого столбца.

```csharp
[Obsolete("Use Column.GetStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Style Style { get; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого, пожалуйста, используйте метод Column.GetStyle() для получения стиля по умолчанию этой колонки. Это свойство будет удалено через 12 месяцев, начиная с декабря 2022 года. Компания Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnPropertyStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить доступ к первой колонке
            Column column = worksheet.Cells.Columns[0];
            
            // Получить текущий стиль с помощью свойства Style
            Style originalStyle = column.Style;
            Console.WriteLine("Original column style - Background: " + originalStyle.BackgroundColor);
            
            // Создать новый стиль и изменить свойства
            Style newStyle = workbook.CreateStyle();
            newStyle.BackgroundColor = Color.LightBlue;
            newStyle.Font.IsBold = true;
            newStyle.HorizontalAlignment = TextAlignmentType.Center;
            
            // Применить новый стиль к колонке
            column.SetStyle(newStyle);
            
            // Добавить данные для демонстрации применения стиля
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue("Data 2");
            
            // Проверить изменения стиля
            Console.WriteLine("New column style applied - Background: " + column.GetStyle().BackgroundColor);
            
            // Сохранить с корректировкой ширины колонок
            column.Width = 15;
            workbook.Save("ColumnStyleDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


