---
title: "Класс GroupFill"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.GroupFill. Представляет формат заливки, который должен наследовать свойства заливки группы"
type: docs
url: /ru/net/aspose.cells.drawing/groupfill/
---
## GroupFill class

Представляет, что данный формат заливки должен наследовать свойства заливки группы.

```csharp
public class GroupFill : Fill
```

## Методы

| Имя | Описание |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Унаследовано от [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Получает хеш-код.(Унаследовано от [`Fill`](../fill/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassGroupFillDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // GroupFill не предоставляет публичный конструктор без параметров.
                // Для демонстрационных целей мы получаем ссылку (null) на тип.
                GroupFill groupFill = null;

                // Покажите, что переменная типа GroupFill существует.
                Console.WriteLine($"GroupFill variable declared. Type: {typeof(GroupFill).FullName}");

                // Сохраните книгу (даже если мы её не изменяли, это демонстрирует полный рабочий процесс)
                workbook.Save("GroupFillDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with GroupFill: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


