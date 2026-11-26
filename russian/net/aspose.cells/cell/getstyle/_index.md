---
title: "Cell.GetStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Получает стиль ячейки"
type: docs
url: /ru/net/aspose.cells/cell/getstyle/
---
## GetStyle() {#getstyle}

Получает стиль ячейки.

```csharp
public Style GetStyle()
```

### Возвращаемое значение

Объект Style.

### Примечания

Чтобы изменить стиль ячейки, пожалуйста, вызовите метод Cell.SetStyle() после изменения возвращённого объекта стиля. Этот метод такой же, как `GetStyle` с истинным значением параметра.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установите различные вертикальные выравнивания для ячеек
            cells["A1"].PutValue("Bottom Alignment");
            cells["A1"].GetStyle().VerticalAlignment = TextAlignmentType.Bottom;

            cells["A2"].PutValue("Center Alignment");
            cells["A2"].GetStyle().VerticalAlignment = TextAlignmentType.Center;

            cells["A3"].PutValue("Distributed Alignment");
            cells["A3"].GetStyle().VerticalAlignment = TextAlignmentType.Distributed;

            cells["A4"].PutValue("Justify Alignment");
            cells["A4"].GetStyle().VerticalAlignment = TextAlignmentType.Justify;

            cells["A5"].PutValue("Top Alignment");
            cells["A5"].GetStyle().VerticalAlignment = TextAlignmentType.Top;

            // Продемонстрировать метод GetStyle()
            Console.WriteLine("A1 Vertical Alignment: " + cells["A1"].GetStyle().VerticalAlignment);
            Console.WriteLine("A2 Vertical Alignment: " + cells["A2"].GetStyle().VerticalAlignment);
            Console.WriteLine("A3 Vertical Alignment: " + cells["A3"].GetStyle().VerticalAlignment);
            Console.WriteLine("A4 Vertical Alignment: " + cells["A4"].GetStyle().VerticalAlignment);
            Console.WriteLine("A5 Vertical Alignment: " + cells["A5"].GetStyle().VerticalAlignment);
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetStyle(bool) {#getstyle_1}

Если checkBorders истинно, проверяет, повлияют ли границы других ячеек на стиль этой ячейки.

```csharp
public Style GetStyle(bool checkBorders)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| checkBorders | Boolean | Проверьте границы других ячеек |

### Возвращаемое значение

Объект Style.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetStyleWithBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получите доступ к ячейке и задайте некоторые примерные данные
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue(123.456);

            // Получите стиль ячейки без наследования от строки/столбца (параметр false)
            Style style = cell.GetStyle(false);
            
            // Изменить стиль
            style.Custom = "0.000";
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.None;

            // Применить изменённый стиль к ячейке
            cell.SetStyle(style);

            // Проверьте изменения стиля
            Console.WriteLine("Number Format: " + cell.GetStyle(false).Custom);
            Console.WriteLine("Top Border Style: " + cell.GetStyle(false).Borders[BorderType.TopBorder].LineStyle);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


