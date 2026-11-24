---
title: "WorkbookDesigner.Workbook"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookDesigner-Eigenschaft. Ruft das Workbook-Objekt ab und legt es fest"
type: docs
url: /de/net/aspose.cells/workbookdesigner/workbook/
---
## WorkbookDesigner.Workbook property

Ruft das `Workbook`-Objekt ab und legt es fest.

```csharp
public Workbook Workbook { get; set; }
```

### Beispiele

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
            // Erstelle einen neuen WorkbookDesigner
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // Setze die Workbook-Eigenschaft mit einer neuen Arbeitsmappe
            designer.Workbook = new Workbook();
            
            // Füge ein Arbeitsblatt und einige Vorlagenmarker hinzu
            Worksheet worksheet = designer.Workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("&Person.Name");
            worksheet.Cells["B1"].PutValue("&Person.Age");

            // Datenquelle erstellen
            List<Person1> persons = new List<Person1>
            {
                new Person1("John", 25),
                new Person1("Mary", 30)
            };

            // Setze Datenquelle und verarbeite
            designer.SetDataSource("Person", persons);
            designer.Process();

            // Ergebnisse ausgeben
            Console.WriteLine("A2: " + worksheet.Cells["A2"].StringValue); // Should output "John"
            Console.WriteLine("B2: " + worksheet.Cells["B2"].IntValue);   // Should output 25
            Console.WriteLine("A3: " + worksheet.Cells["A3"].StringValue); // Should output "Mary"
            Console.WriteLine("B3: " + worksheet.Cells["B3"].IntValue);   // Should output 30

            // Speichere die Arbeitsmappe
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Workbook](../../workbook/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


