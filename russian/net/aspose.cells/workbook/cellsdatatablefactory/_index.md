---
title: "Workbook.CellsDataTableFactory"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Workbook. Возвращает фабрику для создания ICellsDataTable из пользовательских объектов"
type: docs
url: /ru/net/aspose.cells/workbook/cellsdatatablefactory/
---
## Workbook.CellsDataTableFactory property

Получает фабрику для создания ICellsDataTable из пользовательских объектов

```csharp
public CellsDataTableFactory CellsDataTableFactory { get; }
```

### Примеры

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomData
    {
        public int Id { get; set; }
        public string Name { get; set; }
        public int Age { get; set; }
    }

    public class WorkbookPropertyCellsDataTableFactoryDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            List<CustomData> dataList = new List<CustomData>
            {
                new CustomData { Id = 1, Name = "John Doe", Age = 30 },
                new CustomData { Id = 2, Name = "Jane Smith", Age = 25 },
                new CustomData { Id = 3, Name = "Sam Brown", Age = 35 }
            };

            // Получить CellsDataTableFactory из свойства Workbook
            CellsDataTableFactory factory = workbook.CellsDataTableFactory;

            // Создать таблицу данных из списка
            ICellsDataTable dataTable = factory.GetInstance(dataList);

            // Импортировать данные в лист
            sheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

            // Сохраните результаты
            workbook.Save("CellsDataTableFactoryDemo.xlsx");
        }
    }
}
```

### См. также

* class [CellsDataTableFactory](../../cellsdatatablefactory/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


