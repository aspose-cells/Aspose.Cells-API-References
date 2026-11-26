---
title: "TableStyleElement.GetElementStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод TableStyleElement. Получает стиль элемента"
type: docs
url: /ru/net/aspose.cells.tables/tablestyleelement/getelementstyle/
---
## TableStyleElement.GetElementStyle method

Возвращает стиль элемента.

```csharp
public Style GetElementStyle()
```

### Возвращаемое значение

Возвращает объект [`Style`](../../../aspose.cells/style/).

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleElementMethodGetElementStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);
            
            // Создать таблицу
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            
            // Получить стиль таблицы из коллекции стилей таблицы рабочей книги
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            TableStyle style = tableStyles[0];
            table.TableStyleName = style.Name;
            
            // Получить доступ к полному элементу стиля таблицы
            TableStyleElement element = style.TableStyleElements[TableStyleElementType.WholeTable];
            
            // Получить стиль элемента
            Style tableStyle = element.GetElementStyle();
            
            // Изменить свойства стиля
            tableStyle.Font.Name = "Arial";
            tableStyle.Font.Size = 12;
            tableStyle.Font.IsBold = true;
            tableStyle.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            tableStyle.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            tableStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            tableStyle.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            
            // Установить изменённый стиль обратно
            element.SetElementStyle(tableStyle);
            
            // Сохраните книгу
            workbook.Save("TableStyleElementDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../../aspose.cells/style/)
* class [TableStyleElement](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


