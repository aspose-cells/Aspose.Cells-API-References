---
title: "RowCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RowCollection. Возвращает объект Row по заданному индексу строки. Объект Row с указанным индексом будет создан, если он ранее не существовал."
type: docs
url: /ru/net/aspose.cells/rowcollection/item/
---
## RowCollection indexer

Возвращает объект [`Row`](../../row/) по заданному индексу строки. Объект Row с указанным индексом будет создан, если он ранее не существовал.

```csharp
public Row this[int rowIndex] { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установить стандартную ширину столбцов
            cells.StandardWidth = 20.0;

            // Получайте доступ к строкам и задавайте их стиль с помощью свойства Item
            for (int i = 0; i < 5; i++)
            {
                Row row = cells.Rows[i]; // Using Item property
                Style rowStyle = workbook.CreateStyle();
                rowStyle.Font.IsBold = true;
                rowStyle.Font.Color = System.Drawing.Color.Blue;
                row.ApplyStyle(rowStyle, new StyleFlag { Font = true });
                
                // Получайте доступ к ячейке в строке и задавайте её стиль
                Cell cell = cells[i, i]; // Using Cells indexer instead of row[i]
                cell.PutValue($"Row {i}, Col {i}");
                Style cellStyle = workbook.CreateStyle();
                cellStyle.BackgroundColor = System.Drawing.Color.LightYellow;
                cell.SetStyle(cellStyle);
            }

            // Сохраните книгу
            workbook.Save("RowCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### См. также

* class [Row](../../row/)
* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


