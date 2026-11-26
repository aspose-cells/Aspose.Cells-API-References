---
title: "Workbook.ChangePalette"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Изменяет палитру для таблицы в указанном индексе"
type: docs
url: /ru/net/aspose.cells/workbook/changepalette/
---
## Workbook.ChangePalette method

Изменяет палитру электронных таблиц в указанном индексе.

```csharp
public void ChangePalette(Color color, int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| цвет | Color | Структура Color. |
| индекс | Int32 | Индекс палитры, 0 - 55. |

### Примечания

Палитра содержит 56 элементов, каждый представлен RGB‑значением.

Если установить цвет, которого нет в палитре, он не будет применён.

Поэтому, если вы хотите задать пользовательский цвет, сначала измените палитру.

Ниже представлена стандартная цветовая палитра.

| **Color** | **Red** | **Зелёный** | **Синий** |
| --- | --- | --- | --- |
| Черный | 0 | 0 | 0 |
| Белый | 255 | 255 | 255 |
| Красный | 255 | 0 | 0 |
| Лаймовый | 0 | 255 | 0 |
| Синий | 0 | 0 | 255 |
| Желтый | 255 | 255 | 0 |
| Малиновый | 255 | 0 | 255 |
| Голубой | 0 | 255 | 255 |
| Бордовый | 128 | 0 | 0 |
| Зеленый | 0 | 128 | 0 |
| Темно-синий | 0 | 0 | 128 |
| Оливковый | 128 | 128 | 0 |
| Фиолетовый | 128 | 0 | 128 |
| Бирюзовый | 0 | 128 | 128 |
| Серебряный | 192 | 192 | 192 |
| Серый | 128 | 128 | 128 |
| Color17 | 153 | 153 | 255 |
| Color18 | 153 | 51 | 102 |
| Color19 | 255 | 255 | 204 |
| Color20 | 204 | 255 | 255 |
| Color21 | 102 | 0 | 102 |
| Color22 | 255 | 128 | 128 |
| Color23 | 0 | 102 | 204 |
| Color24 | 204 | 204 | 255 |
| Color25 | 0 | 0 | 128 |
| Color26 | 255 | 0 | 255 |
| Color27 | 255 | 255 | 0 |
| Color28 | 0 | 255 | 255 |
| Color29 | 128 | 0 | 128 |
| Color30 | 128 | 0 | 0 |
| Color31 | 0 | 128 | 128 |
| Color32 | 0 | 0 | 255 |
| Color33 | 0 | 204 | 255 |
| Color34 | 204 | 255 | 255 |
| Color35 | 204 | 255 | 204 |
| Color36 | 255 | 255 | 153 |
| Color37 | 153 | 204 | 255 |
| Color38 | 255 | 153 | 204 |
| Color39 | 204 | 153 | 255 |
| Color40 | 255 | 204 | 153 |
| Color41 | 51 | 102 | 255 |
| Color42 | 51 | 204 | 204 |
| Color43 | 153 | 204 | 0 |
| Color44 | 255 | 204 | 0 |
| Color45 | 255 | 153 | 0 |
| Color46 | 255 | 102 | 0 |
| Color47 | 102 | 102 | 153 |
| Color48 | 150 | 150 | 150 |
| Color49 | 0 | 51 | 102 |
| Color50 | 51 | 153 | 102 |
| Color51 | 0 | 51 | 0 |
| Color52 | 51 | 51 | 0 |
| Color53 | 153 | 51 | 0 |
| Color54 | 153 | 51 | 102 |
| Color55 | 51 | 51 | 153 |
| Color56 | 51 | 51 | 51 |

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodChangePaletteWithColorInt32Demo
    {
        public static void Run()
        {
            // Создать экземпляр рабочей книги
            Workbook workbook = new Workbook();
            
            // Изменить цвет палитры в индексе 55
            Color newColor = Color.FromArgb(255, 250, 223);
            workbook.ChangePalette(newColor, 55);

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать стиль с изменённым цветом палитры
            Style style = workbook.CreateStyle();
            style.ForegroundColor = newColor;
            style.Pattern = BackgroundType.Solid;

            // Применить стиль к ячейке
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Palette Color Demo");
            cell.SetStyle(style);

            // Сохраните книгу
            workbook.Save("ChangePaletteDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


