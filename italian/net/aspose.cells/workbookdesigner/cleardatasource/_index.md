---
title: "WorkbookDesigner.ClearDataSource"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WorkbookDesigner. Cancella tutte le origini dati"
type: docs
url: /it/net/aspose.cells/workbookdesigner/cleardatasource/
---
## WorkbookDesigner.ClearDataSource method

Cancella tutte le origini dati.

```csharp
public void ClearDataSource()
```

### Esempi

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

            // Crea dati di esempio
            List<Person> persons = new List<Person>
            {
                new Person("John", 30),
                new Person("Mary", 25),
                new Person("Peter", 35)
            };

            // Configura i marcatori intelligenti
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("&=Person.Name");
            worksheet.Cells["B2"].PutValue("&=Person.Age");

            // Prima associazione dati
            designer.SetDataSource("Person", persons);
            designer.Process();

            // Cancella l'origine dati e ricollega
            designer.ClearDataSource();
            designer.SetDataSource("Person", persons);
            designer.Process();

            // Salva il risultato
            designer.Workbook.Save("ClearedDataSourceOutput.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


