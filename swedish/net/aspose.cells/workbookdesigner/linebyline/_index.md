---
title: "WorkbookDesigner.LineByLine"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookDesigner-egenskap. Anger om bearbetning av smarta markörer sker rad för rad"
type: docs
url: /sv/net/aspose.cells/workbookdesigner/linebyline/
---
## WorkbookDesigner.LineByLine property

Anger om bearbetning av smarta markörer sker rad för rad.

```csharp
[Obsolete("Use range smart markers instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool LineByLine { get; set; }
```

### Anmärkningar

Standardvärdet är true. Om False måste mallfilen innehålla ett område som heter "_CellsSmartMarkers".

OBS: Denna klass är nu föråldrad. Använd i stället smarta markörer för område. Denna egenskap kommer att tas bort 12 månader senare från och med juli 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerPropertyLineByLineDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok med smarta markörer
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Ställ in smarta markörer i kalkylbladet
            ws.Cells["A1"].PutValue("&RootData.Name");
            ws.Cells["A2"].PutValue("&RootData.Age");
            ws.Cells["A3"].PutValue("&RootData.Department");
            
            // Skapa exempeldata
            var employee = new EmployeeData
            {
                Name = "John Doe",
                Age = 35,
                Department = "Sales"
            };
            
            List<EmployeeData> employees = new List<EmployeeData> { employee };

            // Bearbeta med LineByLine satt till false
            WorkbookDesigner designer = new WorkbookDesigner
            {
                Workbook = wb,
                LineByLine = false // This is the key property being demonstrated
            };
            
            designer.SetDataSource("RootData", employees);
            designer.Process();

            // Spara resultatet
            wb.Save("output.xlsx");
            
            Console.WriteLine("Workbook processed with LineByLine=false. Output saved to output.xlsx");
        }
    }

    // Enkel dataklass för demonstration
    public class EmployeeData
    {
        public string Name { get; set; }
        public int Age { get; set; }
        public string Department { get; set; }
    }
}
```

### Se även

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


