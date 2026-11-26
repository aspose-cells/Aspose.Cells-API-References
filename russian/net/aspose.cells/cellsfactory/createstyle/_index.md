---
title: "CellsFactory.CreateStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CellsFactory. Создаёт новый стиль"
type: docs
url: /ru/net/aspose.cells/cellsfactory/createstyle/
---
## CellsFactory.CreateStyle method

Создаёт новый стиль.

```csharp
public Style CreateStyle()
```

### Возвращаемое значение

Возвращает объект стиля.

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellsFactoryMethodCreateStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Создайте стиль с помощью CellsFactory
            Style style = new CellsFactory().CreateStyle();
            
            // Установите свойства границы для стиля
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thick, Color.Black);
            
            // Применить стиль к ячейке
            workbook.Worksheets[0].Cells["A1"].Value = "Hello World";
            workbook.Worksheets[0].Cells["A1"].SetStyle(style);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [CellsFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


