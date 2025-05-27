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
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectReferencePropertyExtendedLibidDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook targetWorkbook = new Workbook();
            
            // Clear existing references
            targetWorkbook.VbaProject.References.Clear();

            // Add a control reference with ExtendedLibid
            string name = "ExampleControl";
            string libid = "{00000000-0000-0000-0000-000000000000}";
            string twiddledLibid = "{11111111-1111-1111-1111-111111111111}";
            string extendedLibid = "ExtendedID123";

            targetWorkbook.VbaProject.References.AddControlRefrernce(
                name, 
                libid, 
                twiddledLibid, 
                extendedLibid);

            // Verify and output the reference count
            Console.WriteLine($"References count: {targetWorkbook.VbaProject.References.Count}");
            
            // Save the workbook
            targetWorkbook.Save("output.xlsm");
        }
    }
}
```

### See Also

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


