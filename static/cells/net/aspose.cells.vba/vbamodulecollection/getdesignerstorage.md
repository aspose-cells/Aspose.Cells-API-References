##VbaModuleCollection.GetDesignerStorage
VbaModuleCollection method. Represents the data of Designer
## VbaModuleCollection.GetDesignerStorage method
Represents the data of Designer.
```csharp
public byte[] GetDesignerStorage(string name)
```
### Remarks
We do not support to parse them. Just only for copying.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;
namespace AsposeCellsExamples
{
public class VbaModuleCollectionMethodGetDesignerStorageWithStringDemo
{
public static void Run()
{
// Create a workbook with VBA project
Workbook workbook = new Workbook();
// Add a designer module
int index = workbook.VbaProject.Modules.Add(VbaModuleType.Designer, "TestForm");
// Get designer storage (will be null initially)
byte[] storage = workbook.VbaProject.Modules.GetDesignerStorage("TestForm");
Console.WriteLine("Initial designer storage: " + (storage == null ? "null" : "exists"));
// Add some designer storage data
byte[] sampleData = new byte[] { 0x01, 0x02, 0x03 };
workbook.VbaProject.Modules.AddDesignerStorage("TestForm", sampleData);
// Get and display the designer storage
storage = workbook.VbaProject.Modules.GetDesignerStorage("TestForm");
Console.WriteLine("Storage after adding: " + (storage == null ? "null" : BitConverter.ToString(storage)));
}
}
}
```
### See Also
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
