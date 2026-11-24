---
title: "WorkbookDesigner.ClearDataSource"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookDesigner-Methode. Löscht alle Datenquellen"
type: docs
url: /de/net/aspose.cells/workbookdesigner/cleardatasource/
---
## WorkbookDesigner.ClearDataSource method

Löscht alle Datenquellen.

```csharp
public void ClearDataSource()
```

### Beispiele

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

            // Erstelle Beispieldaten
            List<Person> persons = new List<Person>
            {
                new Person("John", 30),
                new Person("Mary", 25),
                new Person("Peter", 35)
            };

            // Richte Smartmarker ein
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("&=Person.Name");
            worksheet.Cells["B2"].PutValue("&=Person.Age");

            // Erste Datenbindung
            designer.SetDataSource("Person", persons);
            designer.Process();

            // Datenquelle löschen und erneut binden
            designer.ClearDataSource();
            designer.SetDataSource("Person", persons);
            designer.Process();

            // Ergebnis speichern
            designer.Workbook.Save("ClearedDataSourceOutput.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


