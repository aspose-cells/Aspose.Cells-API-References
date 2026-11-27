---
title: "WorkbookDesigner.Workbook"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookDesigner egenskap. Hämtar och anger Workbook-objektet"
type: docs
url: /sv/net/aspose.cells/workbookdesigner/workbook/
---
## WorkbookDesigner.Workbook property

Hämtar och anger `Workbook`-objektet.

```csharp
public Workbook Workbook { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsboksdesigner
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // Ställ in arbetsboksegenskapen med en ny arbetsbok
            designer.Workbook = new Workbook();
            
            // Lägg till ett kalkylblad och några mallmarkörer
            Worksheet worksheet = designer.Workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("&Person.Name");
            worksheet.Cells["B1"].PutValue("&Person.Age");

            // Skapa datakälla
            List<Person1> persons = new List<Person1>
            {
                new Person1("John", 25),
                new Person1("Mary", 30)
            };

            // Ange datakälla och bearbeta
            designer.SetDataSource("Person", persons);
            designer.Process();

            // Skriv ut resultat
            Console.WriteLine("A2: " + worksheet.Cells["A2"].StringValue); // Should output "John"
            Console.WriteLine("B2: " + worksheet.Cells["B2"].IntValue);   // Should output 25
            Console.WriteLine("A3: " + worksheet.Cells["A3"].StringValue); // Should output "Mary"
            Console.WriteLine("B3: " + worksheet.Cells["B3"].IntValue);   // Should output 30

            // Spara arbetsboken
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Workbook](../../workbook/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


