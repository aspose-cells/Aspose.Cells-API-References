---
title: WorkbookDesigner.VariablesWorksheetName
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner property. Gets and sets the name of the worksheet which contains variables smart marker
type: docs
url: /net/aspose.cells/workbookdesigner/variablesworksheetname/
---
## WorkbookDesigner.VariablesWorksheetName property

Gets and sets the name of the worksheet which contains variables smart marker.

```csharp
public string VariablesWorksheetName { get; set; }
```

### Examples

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
                // Create a new workbook
                Workbook workbook = new Workbook();

                // Add a worksheet named "Variables" to demonstrate the property
                Worksheet variablesSheet = workbook.Worksheets.Add("Variables");
                variablesSheet.Cells["A1"].PutValue("Variable1");
                variablesSheet.Cells["B1"].PutValue("Value1");

                // Create a WorkbookDesigner instance
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // Display the current VariablesWorksheetName value
                Console.WriteLine("Initial VariablesWorksheetName: " + designer.VariablesWorksheetName);

                // Set a new value for VariablesWorksheetName
                designer.VariablesWorksheetName = "Variables";
                Console.WriteLine("Updated VariablesWorksheetName: " + designer.VariablesWorksheetName);

                // Add another worksheet with smart markers
                Worksheet templateSheet = workbook.Worksheets.Add("Template");
                templateSheet.Cells["A1"].PutValue("&=$Variable1");

                // Process the smart markers
                designer.Process();

                // Save the workbook
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

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


