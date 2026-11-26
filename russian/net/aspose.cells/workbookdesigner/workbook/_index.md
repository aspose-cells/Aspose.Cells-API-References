---
title: "WorkbookDesigner.Workbook"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookDesigner. Получает и задает объект Workbook"
type: docs
url: /ru/net/aspose.cells/workbookdesigner/workbook/
---
## WorkbookDesigner.Workbook property

Получает и задает объект `Workbook`.

```csharp
public Workbook Workbook { get; set; }
```

### Примеры

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Person1
    {
        public string Name { get; set; }
        public int Age { get; set; }

        public Person1(string name, int age)
        {
            Name = name;
            Age = age;
        }
    }

    public class WorkbookDesignerPropertyWorkbookDemo
    {
        public static void Run()
        {
            // Создать новый дизайнер рабочей книги
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // Установить свойство workbook новым объектом Workbook
            designer.Workbook = new Workbook();
            
            // Добавить лист и несколько маркеров шаблона
            Worksheet worksheet = designer.Workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("&Person.Name");
            worksheet.Cells["B1"].PutValue("&Person.Age");

            // Создайте источник данных
            List<Person1> persons = new List<Person1>
            {
                new Person1("John", 25),
                new Person1("Mary", 30)
            };

            // Установите источник данных и выполните обработку
            designer.SetDataSource("Person", persons);
            designer.Process();

            // Вывести результаты
            Console.WriteLine("A2: " + worksheet.Cells["A2"].StringValue); // Should output "John"
            Console.WriteLine("B2: " + worksheet.Cells["B2"].IntValue);   // Should output 25
            Console.WriteLine("A3: " + worksheet.Cells["A3"].StringValue); // Should output "Mary"
            Console.WriteLine("B3: " + worksheet.Cells["B3"].IntValue);   // Should output 30

            // Сохраните книгу
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Workbook](../../workbook/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


