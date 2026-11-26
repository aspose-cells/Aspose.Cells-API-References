---
title: "Класс CellsFactory"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.CellsFactory класс. Утилита для создания экземпляров классов модели Cells."
type: docs
url: /ru/net/aspose.cells/cellsfactory/
---
## CellsFactory class

Утилита для создания экземпляров классов модели Cells.

```csharp
public class CellsFactory
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [CellsFactory](cellsfactory/)() | Конструктор по умолчанию. |

## Методы

| Имя | Описание |
| --- | --- |
| [CreateStyle](../../aspose.cells/cellsfactory/createstyle/)() | Создаёт новый стиль. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsFactoryDemo
    {
        public static void CellsFactoryExample()
        {
            // Создать новый экземпляр CellsFactory
            CellsFactory factory = new CellsFactory();

            // Использовать фабрику для создания нового Style
            Style style = factory.CreateStyle();

            // Настроить стиль
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;

            // Создать новую книгу и лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Применить стиль к конкретной ячейке
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Styled Cell");
            cell.SetStyle(style);

            // Сохранить книгу в файл
            workbook.Save("CellsFactoryExample.xlsx");
            workbook.Save("CellsFactoryExample.pdf");
            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


