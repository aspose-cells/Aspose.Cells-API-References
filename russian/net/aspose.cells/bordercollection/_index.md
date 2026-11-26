---
title: "Класс BorderCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.BorderCollection. Инкапсулирует коллекцию объектов Border"
type: docs
url: /ru/net/aspose.cells/bordercollection/
---
## BorderCollection class

Инкапсулирует коллекцию объектов [`Border`](../border/).

```csharp
public class BorderCollection
```

## Свойства

| Имя | Описание |
| --- | --- |
| [DiagonalColor](../../aspose.cells/bordercollection/diagonalcolor/) { get; set; } | Получает или задает Color диагональных линий. |
| [DiagonalStyle](../../aspose.cells/bordercollection/diagonalstyle/) { get; set; } | Получает или задает style диагональных линий. |
| [IsOutline](../../aspose.cells/bordercollection/isoutline/) { get; set; } | Указывает, следует ли применять границы слева, справа, сверху и снизу только к внешним границам диапазона ячеек. Значение по умолчанию — true. |
| [Item](../../aspose.cells/bordercollection/item/) { get; } | Получает элемент [`Border`](../border/) по указанному индексу. |

## Методы

| Имя | Описание |
| --- | --- |
| [SetColor](../../aspose.cells/bordercollection/setcolor/)(Color) | Задает Color всех границ в коллекции. |
| [SetStyle](../../aspose.cells/bordercollection/setstyle/)(CellBorderType) | Задает стиль всех границ в коллекции. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BorderCollectionDemo
    {
        public static void BorderCollectionExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();

            // Добавление нового листа в объект Workbook
            workbook.Worksheets.Add();

            // Получение ссылки на только что добавленный лист путем передачи его индекса листа
            Worksheet worksheet = workbook.Worksheets[0];

            // Доступ к ячейке "A1" листа
            Cell cell = worksheet.Cells["A1"];

            // Добавление некоторого значения в ячейку "A1"
            cell.PutValue("Visit Aspose!");

            // Получение стиля ячейки
            Style style = cell.GetStyle();

            // Установка стиля линии верхней границы
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;

            // Установка цвета верхней границы
            style.Borders[BorderType.TopBorder].Color = Color.Red;

            // Установка стиля линии нижней границы
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thick;

            // Установка цвета нижней границы
            style.Borders[BorderType.BottomBorder].Color = Color.Green;

            // Установка стиля линии левой границы
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dashed;

            // Установка цвета левой границы
            style.Borders[BorderType.LeftBorder].Color = Color.Yellow;

            // Установка стиля линии правой границы
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Dotted;

            // Установка цвета правой границы
            style.Borders[BorderType.RightBorder].Color = Color.Blue;

            // Установка диагональных свойств
            style.Borders.DiagonalColor = Color.Red;
            style.Borders.DiagonalStyle = CellBorderType.Dashed;

            // Применение стиля к ячейке
            cell.SetStyle(style);

            // Сохранение файла Excel
            workbook.Save("BorderCollectionExample.xlsx");
            workbook.Save("BorderCollectionExample.pdf");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


