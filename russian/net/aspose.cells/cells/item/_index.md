---
title: "Cells.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Возвращает элемент Cell по указанному индексу строки и индексу столбца ячейки"
type: docs
url: /ru/net/aspose.cells/cells/item/
---
## Cells indexer (1 of 2)

Получает элемент [`Cell`](../../cell/) по указанному индексу строки ячейки и индексу столбца.

```csharp
public Cell this[int row, int column] { get; }
```

| Параметр | Описание |
| --- | --- |
| строка | Индекс строки. |
| column | Индекс столбца. |

### Возвращаемое значение

Объект [`Cell`](../../cell/).

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Использование свойства Item для доступа и изменения ячеек
            cells[0, 0].PutValue("Hello");
            cells[1, 0].PutValue("World");
            
            // Использование свойства Style через Cells
            Style style1 = cells[0, 0].GetStyle();
            style1.Font.IsBold = true;
            cells[0, 0].SetStyle(style1);

            Style style2 = cells[1, 0].GetStyle();
            style2.Font.Color = System.Drawing.Color.Red;
            cells[1, 0].SetStyle(style2);

            // Сохраните книгу
            workbook.Save("CellsPropertyItemDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Cells indexer (2 of 2)

Получает элемент [`Cell`](../../cell/) по указанному имени ячейки.

```csharp
public Cell this[string cellName] { get; }
```

| Параметр | Описание |
| --- | --- |
| cellName | Имя ячейки, включая её букву столбца и номер строки, например A5. |

### Возвращаемое значение

Объект [`Cell`](../../cell/)

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyItemDemo1
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить доступ к коллекции ячеек
            Cells cells = worksheet.Cells;
            
            // Установить значения, используя свойство Item
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            
            // Установить значения в диапазоне, используя свойство Item
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(25);
            
            // Получать и изменять свойства ячейки с помощью Item
            Cell cell = cells["B1"];
            Style style = cell.GetStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);
            
            // Сохраните книгу
            workbook.Save("CellsPropertyItemDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


