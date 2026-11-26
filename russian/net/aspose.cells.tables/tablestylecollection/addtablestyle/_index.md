---
title: "TableStyleCollection.AddTableStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод TableStyleCollection. Добавляет пользовательский стиль таблицы"
type: docs
url: /ru/net/aspose.cells.tables/tablestylecollection/addtablestyle/
---
## TableStyleCollection.AddTableStyle method

Добавляет пользовательский стиль таблицы.

```csharp
public int AddTableStyle(string name)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя стиля таблицы. |

### Возвращаемое значение

Индекс стиля таблицы.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleCollectionMethodAddTableStyleWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать примерные данные
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[0, i].PutValue("Header " + (i + 1));
                for (int row = 1; row < 6; row++)
                {
                    worksheet.Cells[row, i].PutValue(row * (i + 1));
                }
            }

            // Создать пользовательский стиль таблицы
            string styleName = "MyCustomStyle";
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            int styleIndex = tableStyles.AddTableStyle(styleName);
            TableStyle tableStyle = tableStyles[styleIndex];

            // Оформить строку заголовка
            Style headerStyle = workbook.CreateStyle();
            headerStyle.Font.IsBold = true;
            headerStyle.ForegroundColor = System.Drawing.Color.LightBlue;
            headerStyle.Pattern = BackgroundType.Solid;

            tableStyle.TableStyleElements.Add(TableStyleElementType.HeaderRow);
            TableStyleElement headerElement = tableStyle.TableStyleElements[TableStyleElementType.HeaderRow];
            headerElement.SetElementStyle(headerStyle);

            // Оформить первый столбец
            Style firstColStyle = workbook.CreateStyle();
            firstColStyle.Font.Color = System.Drawing.Color.Red;

            tableStyle.TableStyleElements.Add(TableStyleElementType.FirstColumn);
            TableStyleElement firstColElement = tableStyle.TableStyleElements[TableStyleElementType.FirstColumn];
            firstColElement.SetElementStyle(firstColStyle);

            // Создать таблицу с пользовательским стилем
            int tableIndex = worksheet.ListObjects.Add(0, 0, 5, 4, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.TableStyleName = styleName;
            table.ShowTableStyleFirstColumn = true;

            workbook.Save("CustomTableStyleDemo.xlsx");
        }
    }
}
```

### См. также

* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


