---
title: "TableStyle.TableStyleElements"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TableStyle. Получает все элементы стиля таблицы"
type: docs
url: /ru/net/aspose.cells.tables/tablestyle/tablestyleelements/
---
## TableStyle.TableStyleElements property

Получает все элементы стиля таблицы.

```csharp
public TableStyleElementCollection TableStyleElements { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStylePropertyTableStyleElementsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать примерные данные для таблицы
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Создать таблицу
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.ShowTableStyleFirstColumn = true;

            // Получить стиль таблицы (использовать существующий стиль вместо создания нового)
            TableStyle style = workbook.Worksheets.TableStyles[0];

            // Изменить элементы стиля таблицы
            TableStyleElement wholeTableElement = style.TableStyleElements[TableStyleElementType.WholeTable];
            Style wholeTableStyle = wholeTableElement.GetElementStyle();
            wholeTableStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            wholeTableStyle.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;

            // Применить измененный стиль к таблице
            table.TableStyleName = style.Name;

            // Сохраните книгу
            workbook.Save("TableStyleElementsDemo.xlsx");
        }
    }
}
```

### См. также

* class [TableStyleElementCollection](../../tablestyleelementcollection/)
* class [TableStyle](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


