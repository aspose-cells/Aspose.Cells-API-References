---
title: VbaProject.Modules
second_title: Aspose.Cells for .NET API Reference
description: VbaProject property. Gets all VbaModule objects
type: docs
url: /net/aspose.cells.vba/vbaproject/modules/
---
## VbaProject.Modules property

Gets all [`VbaModule`](../../vbamodule/) objects.

```csharp
public VbaModuleCollection Modules { get; }
```

### Examples

```csharp
// Called: VbaModule vbaModule = vbaProject.Modules[index];
public static void VbaProject_Property_Modules()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            
            // Init VBA project
            VbaProject vbaProject = workbook.VbaProject;
            
            // Add a new class module
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "test");
            
            // Get the VBA module
            VbaModule vbaModule = vbaProject.Modules[index];
            
            // Set codes for the module
            vbaModule.Codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub";
            
            // Save the Excel file
            workbook.Save("VbaModuleTypeExample.xlsm");
        }
```

### See Also

* class [VbaModuleCollection](../../vbamodulecollection/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


