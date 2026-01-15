---
title: VbaProjectReference.ExtendedLibid
second_title: Aspose.Cells for .NET API Reference
description: VbaProjectReference property. Gets and sets the extended Libid of the reference
type: docs
url: /net/aspose.cells.vba/vbaprojectreference/extendedlibid/
---
## VbaProjectReference.ExtendedLibid property

Gets and sets the extended Libid of the reference.

```csharp
public string ExtendedLibid { get; set; }
```

### Remarks

Only for control reference.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaProjectReferencePropertyExtendedLibidDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            try
            {
                // Initialize VBA project
                VbaProject vbaProject = workbook.VbaProject;

                // Add a control reference to demonstrate ExtendedLibid
                vbaProject.References.AddControlRefrernce(
                    "SampleControl",
                    "{00020430-0000-0000-C000-000000000046}",
                    "stdole2.tlb",
                    "2.0");

                // Get the first reference
                VbaProjectReference reference = vbaProject.References[0];

                // Display the ExtendedLibid property value
                Console.WriteLine("ExtendedLibid value: " + reference.ExtendedLibid);

                // Demonstrate setting the ExtendedLibid (since it's read/write)
                reference.ExtendedLibid = "3.0";
                Console.WriteLine("Updated ExtendedLibid value: " + reference.ExtendedLibid);

                // Save the workbook
                workbook.Save("ExtendedLibidDemo.xlsm");
                Console.WriteLine("Workbook saved successfully with ExtendedLibid demonstration.");
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

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


