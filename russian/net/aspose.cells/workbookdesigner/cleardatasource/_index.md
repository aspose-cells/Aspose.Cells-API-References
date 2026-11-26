---
title: "WorkbookDesigner.ClearDataSource"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод WorkbookDesigner. Очищает все источники данных"
type: docs
url: /ru/net/aspose.cells/workbookdesigner/cleardatasource/
---
## WorkbookDesigner.ClearDataSource method

Очищает все источники данных.

```csharp
public void ClearDataSource()
```

### Примеры

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Person
    {
        public string Name { get; set; }
        public int Age { get; set; }

        public Person(string name, int age)
        {
            Name = name;
            Age = age;
        }
    }

    public class WorkbookDesignerMethodClearDataSourceDemo
    {
        public static void Run()
        {
            WorkbookDesigner designer = new WorkbookDesigner();
            Worksheet worksheet = designer.Workbook.Worksheets[0];

            // Создать примерные данные
            List<Person> persons = new List<Person>
            {
                new Person("John", 30),
                new Person("Mary", 25),
                new Person("Peter", 35)
            };

            // Настроить умные маркеры
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("&=Person.Name");
            worksheet.Cells["B2"].PutValue("&=Person.Age");

            // Первое привязывание данных
            designer.SetDataSource("Person", persons);
            designer.Process();

            // Очистить источник данных и привязать заново
            designer.ClearDataSource();
            designer.SetDataSource("Person", persons);
            designer.Process();

            // Сохранить результат
            designer.Workbook.Save("ClearedDataSourceOutput.xlsx");
        }
    }
}
```

### См. также

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


