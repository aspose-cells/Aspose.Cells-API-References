---
title: VbaProjectReference.Type
second_title: Aspose.Cells for .NET API Reference
description: VbaProjectReference property. Gets the type of this reference
type: docs
url: /net/aspose.cells.vba/vbaprojectreference/type/
---
## VbaProjectReference.Type property

Gets the type of this reference.

```csharp
public VbaProjectReferenceType Type { get; }
```

### Examples

```csharp
// Called: Console.WriteLine("Reference Type: " + reference.Type);
public static void Property_Type()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();

            // Init VBA project
            VbaProject vbaProject = workbook.VbaProject;

            // Add VBA project reference
            vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");

            // Saving the Excel file
            workbook.Save("VbaProjectReferenceTypeExample.xlsm");

            // Demonstrating the use of VbaProjectReferenceType enum
            VbaProjectReference reference = vbaProject.References[0];
            Console.WriteLine("Reference Type: " + reference.Type);
            Console.WriteLine("Reference Name: " + reference.Name);
            Console.WriteLine("Reference Libid: " + reference.Libid);
        }
```

### See Also

* enum [VbaProjectReferenceType](../../vbaprojectreferencetype/)
* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


