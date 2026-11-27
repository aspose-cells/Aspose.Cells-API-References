---
title: "WorkbookDesigner.ClearDataSource"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookDesigner metod. Rensar alla datakällor"
type: docs
url: /sv/net/aspose.cells/workbookdesigner/cleardatasource/
---
## WorkbookDesigner.ClearDataSource method

Rensar alla datakällor.

```csharp
public void ClearDataSource()
```

### Exempel

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

            // Skapa exempeldata
            List<Person> persons = new List<Person>
            {
                new Person("John", 30),
                new Person("Mary", 25),
                new Person("Peter", 35)
            };

            // Ställ in smarta markörer
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("&=Person.Name");
            worksheet.Cells["B2"].PutValue("&=Person.Age");

            // Första databindning
            designer.SetDataSource("Person", persons);
            designer.Process();

            // Rensa datakälla och återbind
            designer.ClearDataSource();
            designer.SetDataSource("Person", persons);
            designer.Process();

            // Spara resultatet
            designer.Workbook.Save("ClearedDataSourceOutput.xlsx");
        }
    }
}
```

### Se även

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


