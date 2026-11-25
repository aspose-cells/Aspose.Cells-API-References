---
title: "WorkbookDesigner.Workbook"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookDesigner. Ottiene e imposta l'oggetto Workbook"
type: docs
url: /it/net/aspose.cells/workbookdesigner/workbook/
---
## WorkbookDesigner.Workbook property

Ottiene e imposta l'oggetto `Workbook`.

```csharp
public Workbook Workbook { get; set; }
```

### Esempi

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
            // Crea un nuovo designer di cartella di lavoro
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // Imposta la proprietà workbook con una nuova cartella di lavoro
            designer.Workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro e alcuni marcatori del modello
            Worksheet worksheet = designer.Workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("&Person.Name");
            worksheet.Cells["B1"].PutValue("&Person.Age");

            // Crea la fonte dati
            List<Person1> persons = new List<Person1>
            {
                new Person1("John", 25),
                new Person1("Mary", 30)
            };

            // Imposta la fonte dati ed elabora
            designer.SetDataSource("Person", persons);
            designer.Process();

            // Restituisci i risultati
            Console.WriteLine("A2: " + worksheet.Cells["A2"].StringValue); // Should output "John"
            Console.WriteLine("B2: " + worksheet.Cells["B2"].IntValue);   // Should output 25
            Console.WriteLine("A3: " + worksheet.Cells["A3"].StringValue); // Should output "Mary"
            Console.WriteLine("B3: " + worksheet.Cells["B3"].IntValue);   // Should output 30

            // Salva la cartella di lavoro
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Workbook](../../workbook/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


