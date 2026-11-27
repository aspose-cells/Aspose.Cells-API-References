---
title: "WorkbookDesigner.VariablesWorksheetName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookDesigner-egenskap. Hämtar och anger namnet på kalkylbladet som innehåller variabler smart marker"
type: docs
url: /sv/net/aspose.cells/workbookdesigner/variablesworksheetname/
---
## WorkbookDesigner.VariablesWorksheetName property

Hämtar och anger namnet på kalkylbladet som innehåller variabler för smart marker.

```csharp
public string VariablesWorksheetName { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookDesignerPropertyVariablesWorksheetNameDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en ny arbetsbok
                Workbook workbook = new Workbook();

                // Lägg till ett kalkylblad med namnet "Variables" för att demonstrera egenskapen
                Worksheet variablesSheet = workbook.Worksheets.Add("Variables");
                variablesSheet.Cells["A1"].PutValue("Variable1");
                variablesSheet.Cells["B1"].PutValue("Value1");

                // Skapa en WorkbookDesigner‑instans
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // Visa det aktuella värdet för VariablesWorksheetName
                Console.WriteLine("Initial VariablesWorksheetName: " + designer.VariablesWorksheetName);

                // Ange ett nytt värde för VariablesWorksheetName
                designer.VariablesWorksheetName = "Variables";
                Console.WriteLine("Updated VariablesWorksheetName: " + designer.VariablesWorksheetName);

                // Lägg till ett annat kalkylblad med smarta markörer
                Worksheet templateSheet = workbook.Worksheets.Add("Template");
                templateSheet.Cells["A1"].PutValue("&=$Variable1");

                // Bearbeta de smarta markörerna
                designer.Process();

                // Spara arbetsboken
                workbook.Save("VariablesWorksheetNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with VariablesWorksheetName set.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


