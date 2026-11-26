---
title: "Класс TableStyleElement"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Tables.TableStyleElement. Представляет элемент стиля таблицы"
type: docs
url: /ru/net/aspose.cells.tables/tablestyleelement/
---
## TableStyleElement class

Представляет элемент стиля таблицы.

```csharp
public class TableStyleElement
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Size](../../aspose.cells.tables/tablestyleelement/size/) { get; set; } | Количество строк или столбцов в одной полосе чередования. Применяется только когда тип — firstRowStripe, secondRowStripe, firstColumnStripe или secondColumnStripe. |
| [Type](../../aspose.cells.tables/tablestyleelement/type/) { get; } | Возвращает тип элемента. |

## Методы

| Имя | Описание |
| --- | --- |
| [GetElementStyle](../../aspose.cells.tables/tablestyleelement/getelementstyle/)() | Возвращает стиль элемента. |
| [SetElementStyle](../../aspose.cells.tables/tablestyleelement/setelementstyle/)(Style) | Устанавливает стиль элемента. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TablesClassTableStyleElementDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            Style firstColumnStyle = workbook.CreateStyle();
            firstColumnStyle.Pattern = BackgroundType.Solid;
            firstColumnStyle.BackgroundColor = System.Drawing.Color.LightBlue;

            Style lastColumnStyle = workbook.CreateStyle();
            lastColumnStyle.Font.IsBold = true;
            lastColumnStyle.ForegroundColor = System.Drawing.Color.Yellow;
            lastColumnStyle.Pattern = BackgroundType.Solid;

            string tableStyleName = "CustomStyle1";
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            int styleIndex = tableStyles.AddTableStyle(tableStyleName);
            TableStyle tableStyle = tableStyles[styleIndex];

            TableStyleElementCollection elements = tableStyle.TableStyleElements;
            
            int elementIndex = elements.Add(TableStyleElementType.FirstColumn);
            TableStyleElement element = elements[elementIndex];
            element.SetElementStyle(firstColumnStyle);

            elementIndex = elements.Add(TableStyleElementType.LastColumn);
            element = elements[elementIndex];
            element.SetElementStyle(lastColumnStyle);

            Cells cells = workbook.Worksheets[0].Cells;
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue($"Column {i + 1}");
            }
            for (int row = 1; row < 5; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    cells[row, col].PutValue(row * col);
                }
            }

            ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
            int tableIndex = tables.Add(0, 0, 4, 4, true);
            ListObject table = tables[tableIndex];

            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.TableStyleName = tableStyleName;

            workbook.Save("TableStyleElementDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


