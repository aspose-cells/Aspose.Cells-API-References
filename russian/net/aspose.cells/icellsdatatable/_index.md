---
title: "Интерфейс ICellsDataTable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Интерфейс Aspose.Cells.ICellsDataTable. Представляет таблицу данных"
type: docs
url: /ru/net/aspose.cells/icellsdatatable/
---
## ICellsDataTable interface

Представляет таблицу данных.

```csharp
public interface ICellsDataTable
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Columns](../../aspose.cells/icellsdatatable/columns/) { get; } | Получает имя столбцов. |
| [Count](../../aspose.cells/icellsdatatable/count/) { get; } | Получает количество записей. -1 означает неизвестное количество записей. |
| [Item](../../aspose.cells/icellsdatatable/item/) { get; } | Получает данные, хранящиеся в столбце, указанном по индексу. (2 индексатора) |

## Методы

| Имя | Описание |
| --- | --- |
| [BeforeFirst](../../aspose.cells/icellsdatatable/beforefirst/)() | Переместите курсор в начало этого объекта, сразу перед первой строкой. |
| [Next](../../aspose.cells/icellsdatatable/next/)() | Перемещает курсор вниз на одну строку от текущей позиции. |

### Примеры

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassICellsDataTableDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();

            ArrayList dataLists = new ArrayList();
            ArrayList list1 = new ArrayList();
            list1.AddRange(new object[] { "Name", "Age", "Gender" });
            ArrayList list2 = new ArrayList();
            list2.AddRange(new object[] { "Alice", 30, "Female" });
            ArrayList list3 = new ArrayList();
            list3.AddRange(new object[] { "Bob", 25, "Male" });
            ArrayList list4 = new ArrayList();
            list4.AddRange(new object[] { "Charlie", 35, "Male" });
            dataLists.Add(list1);
            dataLists.Add(list2);
            dataLists.Add(list3);
            dataLists.Add(list4);

            ICellsDataTable dt = wb.CellsDataTableFactory.GetInstance(dataLists, true);
            
            wb.Worksheets[0].Cells.ImportData(dt, 0, 0, new ImportTableOptions());
            Console.WriteLine("First worksheet A2 value: " + wb.Worksheets[0].Cells["A2"].StringValue);

            wb.Worksheets.Add();
            wb.Worksheets[1].Cells.ImportArrayList(dataLists, 0, 0, true);
            Console.WriteLine("Second worksheet A3 value: " + wb.Worksheets[1].Cells["A3"].StringValue);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


