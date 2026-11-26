---
title: "Класс DataModel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.DataModels.DataModel. Представляет модель данных"
type: docs
url: /ru/net/aspose.cells.datamodels/datamodel/
---
## DataModel class

Представляет модель данных.

```csharp
public class DataModel
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Relationships](../../aspose.cells.datamodels/datamodel/relationships/) { get; } | Получает все связи таблиц в модели данных. |
| [Tables](../../aspose.cells.datamodels/datamodel/tables/) { get; } | Получает все таблицы в модели данных. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DataModels;
    using System;

    public class DataModelsClassDataModelDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получите DataModel из рабочей книги вместо создания нового экземпляра
            DataModel dataModel = workbook.DataModel;

            // Продемонстрировать доступ к таблицам и связям (только свойства для чтения)
            Console.WriteLine("Number of tables in DataModel: " + dataModel.Tables.Count);
            Console.WriteLine("Number of relationships in DataModel: " + dataModel.Relationships.Count);

            // Примечание: Поскольку Таблицы и Связи являются коллекциями только для чтения,
            // мы можем только получать существующие элементы, но не изменять их напрямую

            // Сохранить рабочую книгу (DataModel обычно используется внутри Aspose.Cells)
            workbook.Save("DataModelDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.DataModels](../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../)


