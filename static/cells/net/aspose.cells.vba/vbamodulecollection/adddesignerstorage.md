##VbaModuleCollection.AddDesignerStorage
VbaModuleCollection method.
## VbaModuleCollection.AddDesignerStorage method
```csharp
public void AddDesignerStorage(string name, byte[] data)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String |  |
| data | Byte[] |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Vba;
using System;
using System.Text;
public class VbaModuleCollectionMethodAddDesignerStorageWithStringByteDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the VBA project
VbaProject vbaProject = workbook.VbaProject;
// Prepare data for designer storage
string storageName = "MyDesignerStorage";
byte[] storageData = Encoding.UTF8.GetBytes("This is designer storage data");
try
{
// Call AddDesignerStorage method
vbaProject.Modules.AddDesignerStorage(storageName, storageData);
Console.WriteLine("Designer storage added successfully");
// Verify the storage was added
byte[] retrievedData = vbaProject.Modules.GetDesignerStorage(storageName);
if (retrievedData != null)
{
Console.WriteLine("Retrieved storage data: " + Encoding.UTF8.GetString(retrievedData));
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing AddDesignerStorage method: {ex.Message}");
}
// Save the workbook
workbook.Save("VbaModuleCollectionMethodAddDesignerStorageWithStringByteDemo.xlsx");
}
}
}
```
### See Also
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
