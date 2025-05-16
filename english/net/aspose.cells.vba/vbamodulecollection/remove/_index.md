---
title: VbaModuleCollection.Remove
second_title: Aspose.Cells for .NET API Reference
description: VbaModuleCollection method. Removes module for a worksheet
type: docs
url: /net/aspose.cells.vba/vbamodulecollection/remove/
---
## Remove(Worksheet) {#remove}

Removes module for a worksheet.

```csharp
public void Remove(Worksheet sheet)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sheet | Worksheet | The worksheet |

### Examples

```csharp
namespace AsposeCellsExamples.VbaModuleCollectionMethodRemoveWithWorksheetDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaModuleCollectionMethodRemoveWithWorksheetDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add a VBA module to the worksheet
            int moduleIndex = workbook.VbaProject.Modules.Add(worksheet);
            
            // Get the VBA module collection
            VbaModuleCollection modules = workbook.VbaProject.Modules;
            
            try
            {
                // Call the Remove method with the worksheet parameter
                modules.Remove(worksheet);
                
                Console.WriteLine("VBA module removed successfully for the specified worksheet.");
                
                // Verify the module was removed
                if (modules.Count == 0)
                {
                    Console.WriteLine("No VBA modules remain in the collection.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Remove method: {ex.Message}");
            }
            
            // Save the result
            workbook.Save("VbaModuleRemoveWithWorksheetDemo.xlsx");
        }
    }
}
```

### See Also

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)

---

## Remove(string) {#remove_1}

Remove the module by the name

```csharp
public void Remove(string name)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String |  |

### Examples

```csharp
// Called: vbaProject.Modules.Remove("TestForm");
public void VbaModuleCollection_Method_Remove()
{
    var source = new Workbook(Constants.sourcePath + "example.xlsm");
    var wb = new Workbook(Constants.sourcePath + "example.xlsm");
    VbaProject vbaProject = wb.VbaProject;
    vbaProject.Modules.Remove("TestForm");
    Assert.IsNull(vbaProject.Modules.GetDesignerStorage("TestForm"));
    vbaProject.Modules.AddDesignerStorage("TestForm", source.VbaProject.Modules.GetDesignerStorage("TestForm"));
    int index = vbaProject.Modules.Add(VbaModuleType.Designer, "TestForm");
    vbaProject.Modules[index].Codes = source.VbaProject.Modules["TestForm"].Codes;
    wb.Save(Constants.destPath + "example.xlsm");
}
```

### See Also

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


