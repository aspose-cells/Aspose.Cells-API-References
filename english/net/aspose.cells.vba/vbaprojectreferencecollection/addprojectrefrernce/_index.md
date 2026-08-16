---
title: VbaProjectReferenceCollection.AddProjectRefrernce
second_title: Aspose.Cells for .NET API Reference
description: VbaProjectReferenceCollection method. Adds a reference to an external VBA project
type: docs
url: /net/aspose.cells.vba/vbaprojectreferencecollection/addprojectrefrernce/
---
## VbaProjectReferenceCollection.AddProjectRefrernce method

Adds a reference to an external VBA project.

```csharp
[Obsolete("Use VbaProjectReferenceCollection.AddProjectReferernce() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AddProjectRefrernce(string name, string absoluteLibid, string relativeLibid)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of reference. |
| absoluteLibid | String | The referenced VBA project's identifier with an absolute path. |
| relativeLibid | String | The referenced VBA project's identifier with an relative path. |

### Remarks

NOTE: This method is now obsolete. Instead, please use VbaProjectReferenceCollection.AddProjectReferernce() method. This method will be removed 12 months later since July 2026. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferenceCollectionMethodAddProjectRefrernceWithStringStringStringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Initialize VBA project
            VbaProject vbaProject = workbook.VbaProject;
            
            // Add a project reference with absolute and relative libids
            vbaProject.References.AddProjectRefrernce("MyProject", "absoluteLibid", "relativeLibid");
            
            // Display reference count
            Console.WriteLine("Total References: " + vbaProject.References.Count);
            
            // Save the workbook
            workbook.Save("VbaProjectReferenceExample.xlsm");
        }
    }
}
```

### See Also

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


