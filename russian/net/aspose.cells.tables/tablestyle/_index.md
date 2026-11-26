---
title: "Класс TableStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Tables.TableStyle. Представляет стиль таблицы"
type: docs
url: /ru/net/aspose.cells.tables/tablestyle/
---
## TableStyle class

Представляет стиль таблицы.

```csharp
public class TableStyle
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Name](../../aspose.cells.tables/tablestyle/name/) { get; } | Получает имя стиля таблицы. |
| [TableStyleElements](../../aspose.cells.tables/tablestyle/tablestyleelements/) { get; } | Получает все элементы стиля таблицы. |

## Методы

| Имя | Описание |
| --- | --- |
| static [Create](../../aspose.cells.tables/tablestyle/create/)(string, WorksheetCollection) | Создает пустой стиль таблицы/сводной таблицы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleDemo
    {
        public static void TableStyleExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Создать стили для первого и последнего столбцов
            Style firstColumnStyle = workbook.CreateStyle();
            firstColumnStyle.Pattern = BackgroundType.Solid;
            firstColumnStyle.BackgroundColor = System.Drawing.Color.Red;

            Style lastColumnStyle = workbook.CreateStyle();
            lastColumnStyle.Font.IsBold = true;
            lastColumnStyle.Pattern = BackgroundType.Solid;
            lastColumnStyle.BackgroundColor = System.Drawing.Color.Red;

            // Определить имя пользовательского стиля таблицы
            string tableStyleName = "Custom1";

            // Получить доступ к коллекции стилей таблицы
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

            // Добавить новый стиль таблицы в коллекцию
            int index1 = tableStyles.AddTableStyle(tableStyleName);
            TableStyle tableStyle = tableStyles[index1];

            // Получить доступ к коллекции элементов стиля таблицы
            TableStyleElementCollection elements = tableStyle.TableStyleElements;

            // Добавить и установить стиль для первого столбца
            index1 = elements.Add(TableStyleElementType.FirstColumn);
            TableStyleElement element = elements[index1];
            element.SetElementStyle(firstColumnStyle);

            // Добавить и установить стиль для последнего столбца
            index1 = elements.Add(TableStyleElementType.LastColumn);
            element = elements[index1];
            element.SetElementStyle(lastColumnStyle);

            // Получить доступ к ячейкам первого листа
            Cells cells = workbook.Worksheets[0].Cells;

            // Заполнить первую строку именами столбцов
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }

            // Заполнить остальные ячейки примерными данными
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Добавить таблицу в лист
            ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Применить пользовательский стиль таблицы к таблице.
            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.TableStyleName = tableStyleName;

            // Сохраните книгу
            workbook.Save("TableStyleExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


