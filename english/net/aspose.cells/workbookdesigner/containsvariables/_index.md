---
title: WorkbookDesigner.ContainsVariables
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner property. Indicates whether the first worksheet contains custom variables
type: docs
url: /net/aspose.cells/workbookdesigner/containsvariables/
---
## WorkbookDesigner.ContainsVariables property

Indicates whether the first worksheet contains custom variables.

```csharp
[Obsolete("Use WorkbookDesigner.VariablesWorksheetName property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ContainsVariables { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use WorkbookDesigner.VariablesWorksheetName property, instead. This property will be removed 3 months later since September 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookDesignerPropertyContainsVariablesDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Create a sample worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to make the example meaningful
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Create a WorkbookDesigner instance
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // Display the current value of the ContainsVariables property
                Console.WriteLine("Initial ContainsVariables value: " + designer.ContainsVariables);

                // Set the ContainsVariables property to true
                designer.ContainsVariables = true;

                // Display the updated value
                Console.WriteLine("Updated ContainsVariables value: " + designer.ContainsVariables);

                // Save the result
                workbook.Save("ContainsVariablesDemo.xlsx");

                Console.WriteLine("ContainsVariables property has been demonstrated");
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


