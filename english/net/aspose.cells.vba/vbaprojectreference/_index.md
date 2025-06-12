---
title: Class VbaProjectReference
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Vba.VbaProjectReference class. Represents the reference of VBA project
type: docs
url: /net/aspose.cells.vba/vbaprojectreference/
---
## VbaProjectReference class

Represents the reference of VBA project.

```csharp
public class VbaProjectReference
```

## Properties

| Name | Description |
| --- | --- |
| [ExtendedLibid](../../aspose.cells.vba/vbaprojectreference/extendedlibid/) { get; set; } | Gets and sets the extended Libid of the reference. |
| [Libid](../../aspose.cells.vba/vbaprojectreference/libid/) { get; set; } | Gets and sets the Libid of the reference. |
| [Name](../../aspose.cells.vba/vbaprojectreference/name/) { get; set; } | Gets and sets the name of the reference. |
| [RelativeLibid](../../aspose.cells.vba/vbaprojectreference/relativelibid/) { get; set; } | Gets and sets the referenced VBA project's identifier with an relative path. |
| [Twiddledlibid](../../aspose.cells.vba/vbaprojectreference/twiddledlibid/) { get; set; } | Gets and sets the twiddled Libid of the reference. |
| [Type](../../aspose.cells.vba/vbaprojectreference/type/) { get; } | Gets the type of this reference. |

## Methods

| Name | Description |
| --- | --- |
| [Copy](../../aspose.cells.vba/vbaprojectreference/copy/)(VbaProjectReference) |  |

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaClassVbaProjectReferenceDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Initialize VBA project
            VbaProject vbaProject = workbook.VbaProject;
            
            // Add registered reference to VBA project
            vbaProject.References.AddRegisteredReference(
                "stdole", 
                "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
            
            // Save the workbook with VBA project
            workbook.Save("output.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


