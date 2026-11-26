---
title: "NameCollection.Filter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод NameCollection. Получает все определённые имена по области"
type: docs
url: /ru/net/aspose.cells/namecollection/filter/
---
## NameCollection.Filter method

Получает все определённые имена по области.

```csharp
public Name[] Filter(NameScopeType type, int sheetIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | NameScopeType | Тип области. |
| sheetIndex | Int32 | Индекс листа. Действует только когда тип области — Worksheet |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodFilterWithNameScopeTypeInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте несколько имён в книгу и листы
            workbook.Worksheets.Names.Add("GlobalName");
            Worksheet worksheet1 = workbook.Worksheets[0];
            workbook.Worksheets.Names.Add("Sheet1Name");
            Worksheet worksheet2 = workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Names.Add("Sheet2Name");

            // Отфильтруйте имена по типу области и индексу листа
            Name[] workbookScopeNames = workbook.Worksheets.Names.Filter(NameScopeType.Workbook, -1);
            Name[] worksheetScopeNames = workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, -1);
            Name[] sheet1Names = workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, 0);

            // Вывести результаты
            Console.WriteLine($"Workbook-scoped names count: {workbookScopeNames.Length}");
            Console.WriteLine($"Worksheet-scoped names count: {worksheetScopeNames.Length}");
            Console.WriteLine($"Sheet1 names count: {sheet1Names.Length}");
        }
    }
}
```

### См. также

* class [Name](../../name/)
* enum [NameScopeType](../../namescopetype/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


