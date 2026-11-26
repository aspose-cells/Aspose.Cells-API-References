---
title: "BorderCollection.SetStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод BorderCollection. Устанавливает стиль всех границ коллекции"
type: docs
url: /ru/net/aspose.cells/bordercollection/setstyle/
---
## BorderCollection.SetStyle method

Задает стиль всех границ в коллекции.

```csharp
public void SetStyle(CellBorderType style)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| стиль | CellBorderType | Стиль границ |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderCollectionMethodSetStyleWithCellBorderTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить ячейку C6 и её стиль
            Cell cell = worksheet.Cells["C6"];
            Style style = cell.GetStyle();

            // Установить цвет и стиль границы
            style.Borders.SetColor(System.Drawing.Color.Red);
            style.Borders.SetStyle(CellBorderType.Thick);

            // Применить стиль к ячейке
            cell.SetStyle(style);

            // Сохраните книгу
            workbook.Save("BorderCollectionMethodSetStyleWithCellBorderTypeDemo_out.xlsx");

            Console.WriteLine("Border style set successfully.");
        }
    }
}
```

### См. также

* enum [CellBorderType](../../cellbordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


