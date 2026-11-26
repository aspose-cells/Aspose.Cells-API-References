---
title: "Класс Row"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Row class. Представляет одну строку в листе"
type: docs
url: /ru/net/aspose.cells/row/
---
## Row class

Представляет одну строку в листе.

```csharp
public class Row : IEnumerable
```

## Свойства

| Имя | Описание |
| --- | --- |
| [FirstCell](../../aspose.cells/row/firstcell/) { get; } | Получает первый объект ячейки в строке. |
| [FirstDataCell](../../aspose.cells/row/firstdatacell/) { get; } | Получает первую непустую ячейку в строке. |
| [GroupLevel](../../aspose.cells/row/grouplevel/) { get; set; } | Получает уровень группы строки. |
| [HasCustomStyle](../../aspose.cells/row/hascustomstyle/) { get; } | Указывает, имеет ли эта строка пользовательские настройки стиля (отличные от значения по умолчанию, унаследованного от книги). |
| [Height](../../aspose.cells/row/height/) { get; set; } | Получает и задает высоту строки в единицах точек. |
| [Index](../../aspose.cells/row/index/) { get; } | Получает индекс этой строки. |
| [IsBlank](../../aspose.cells/row/isblank/) { get; } | Указывает, содержит ли строка какие-либо данные |
| [IsCollapsed](../../aspose.cells/row/iscollapsed/) { get; set; } | является ли строка свернутой |
| [IsHeightMatched](../../aspose.cells/row/isheightmatched/) { get; set; } | Указывает, соответствует ли высота строки текущим настройкам шрифта по умолчанию в рабочей книге. Значение true этого свойства также означает, что высота строки "автоматическая" без пользовательского значения высоты. |
| [IsHidden](../../aspose.cells/row/ishidden/) { get; set; } | Указывает, скрыта ли строка. |
| [Item](../../aspose.cells/row/item/) { get; } | Получает ячейку. |
| [LastCell](../../aspose.cells/row/lastcell/) { get; } | Получает последний объект ячейки в строке. |
| [LastDataCell](../../aspose.cells/row/lastdatacell/) { get; } | Получает последнюю непустую ячейку в строке. |

## Методы

| Имя | Описание |
| --- | --- |
| [ApplyStyle](../../aspose.cells/row/applystyle/)(Style, StyleFlag) | Применяет форматы к целой строке. |
| [CopySettings](../../aspose.cells/row/copysettings/)(Row, bool) | Копирует настройки строки, такие как стиль, высота, видимость и т.д. |
| override [Equals](../../aspose.cells/row/equals/#equals_1)(object) | Проверяет, относится ли этот объект к той же строке, что и другой. |
| [Equals](../../aspose.cells/row/equals/#equals)(Row) | Проверяет, относится ли этот объект к той же строке, что и другой объект строки. |
| [GetCellByIndex](../../aspose.cells/row/getcellbyindex/)(int) | Получить ячейку по конкретному индексу в коллекции ячеек этой строки. |
| [GetCellOrNull](../../aspose.cells/row/getcellornull/)(int) | Получает ячейку или null по указанному индексу. |
| [GetEnumerator](../../aspose.cells/row/getenumerator/#getenumerator)() | Получает перечислитель ячеек |
| [GetEnumerator](../../aspose.cells/row/getenumerator/#getenumerator_1)(bool, bool) | Получает перечислитель, который перебирает ячейки в этой строке. |
| [GetStyle](../../aspose.cells/row/getstyle/)() | Получает стиль этой строки. |
| [SetStyle](../../aspose.cells/row/setstyle/)(Style) | Задает стиль этой строки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;
    using System.Collections;

    public class RowDemo
    {
        public static void RowExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();

            // Получение ссылки на первый лист
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать объект стиля
            Style style = workbook.CreateStyle();

            // Установка фонового цвета в синий
            style.BackgroundColor = Color.Blue;

            // Установка цвета переднего плана в красный
            style.ForegroundColor = Color.Red;

            // Установка фонового узора
            style.Pattern = BackgroundType.DiagonalStripe;

            // Новый флаг стиля
            StyleFlag styleFlag = new StyleFlag();

            // Установить все стили
            styleFlag.All = true;

            // Получить первую строку
            Row row = worksheet.Cells.Rows[0];

            // Применить стиль к первой строке
            row.ApplyStyle(style, styleFlag);

            // Настройка свойств строки
            row.Height = 20.0;
            row.IsHidden = false;
            row.IsCollapsed = false;
            row.GroupLevel = 1;
            row.IsHeightMatched = true;

            // Доступ к ячейкам в строке
            Cell firstCell = row.FirstCell;
            Cell firstDataCell = row.FirstDataCell;
            Cell lastCell = row.LastCell;
            Cell lastDataCell = row.LastDataCell;

            // Проверка, пуста ли строка
            bool isBlank = row.IsBlank;

            // Проверка, имеет ли строка пользовательский стиль
            bool hasCustomStyle = row.HasCustomStyle;

            // Получение индекса строки
            int rowIndex = row.Index;

            // Получение ячейки по индексу
            Cell cellByIndex = row.GetCellByIndex(0);

            // Получение стиля строки
            Style rowStyle = row.GetStyle();

            // Установка стиля строки
            row.SetStyle(rowStyle);

            // Копирование настроек из другой строки
            Row sourceRow = worksheet.Cells.Rows[1];
            row.CopySettings(sourceRow, true);

            // Перебор ячеек в строке
            IEnumerator cellEnumerator = row.GetEnumerator();
            while (cellEnumerator.MoveNext())
            {
                Cell cell = (Cell)cellEnumerator.Current;
                Console.WriteLine(cell.Name + ": " + cell.Value);
            }

            // Сохранение файла Excel
            workbook.Save("RowExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


