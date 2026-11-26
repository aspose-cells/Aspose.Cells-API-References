---
title: "Класс CellsDataTableFactory"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.CellsDataTableFactory. Утилита для построения ICellsDataTable из пользовательских объектов для удобства пользователей"
type: docs
url: /ru/net/aspose.cells/cellsdatatablefactory/
---
## CellsDataTableFactory class

Утилита для создания ICellsDataTable из пользовательских объектов для удобства пользователя.

```csharp
public class CellsDataTableFactory
```

## Методы

| Имя | Описание |
| --- | --- |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance)(double[]) |  |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_6)(ICollection) | Создаёт ICellsDataTable из заданной коллекции. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_3)(int[]) |  |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_8)(object[]) |  |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_1)(double[], bool) | Создаёт ICellsDataTable из заданной последовательности значений double. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_2)(double[], string[]) | Создаёт ICellsDataTable из заданной последовательности значений double. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_7)(ICollection, bool) | Создаёт ICellsDataTable из заданной коллекции. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_4)(int[], bool) | Создаёт ICellsDataTable из заданной последовательности целочисленных значений. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_5)(int[], string[]) | Создаёт ICellsDataTable из заданной последовательности целочисленных значений. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_9)(object[], bool) | Создаёт ICellsDataTable из заданной последовательности объектов. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_10)(object[], string[]) | Создаёт ICellsDataTable из заданной последовательности объектов. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_11)(object[][], bool, string[]) | Создаёт ICellsDataTable из заданной последовательности объектов. |

### Примеры

```csharp
using Aspose.Cells;
using System;
using System.Collections.Generic;

namespace AsposeCellsExamples
{
    public class CellsDataTableFactoryDemo
    {
        public static void RunDemo()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            List<CustomData> dataList = new List<CustomData>
            {
                new CustomData { Id = 1, Name = "John Doe", Age = 30 },
                new CustomData { Id = 2, Name = "Jane Smith", Age = 25 },
                new CustomData { Id = 3, Name = "Sam Brown", Age = 35 }
            };

            // Получить экземпляр CellsDataTableFactory из книги
            CellsDataTableFactory factory = workbook.CellsDataTableFactory;

            // Создать экземпляр ICellsDataTable из пользовательского списка данных
            ICellsDataTable dataTable = factory.GetInstance(dataList);

            // Импортировать таблицу данных в лист, начиная с ячейки A1
            sheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

            // Сохраните книгу
            workbook.Save("CellsDataTableFactoryDemo.xlsx");
            workbook.Save("CellsDataTableFactoryDemo.pdf");
        }
    }

    // Пользовательский класс данных
    public class CustomData
    {
        public int Id { get; set; }
        public string Name { get; set; }
        public int Age { get; set; }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


