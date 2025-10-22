##VbaModuleCollection.AddUserForm
VbaModuleCollection method. Inser user form into VBA Project
## VbaModuleCollection.AddUserForm method
Inser user form into VBA Project.
```csharp
public int AddUserForm(string name, string codes, byte[] designerStorage)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of user form |
| codes | String | The codes for the user form |
| designerStorage | Byte[] | the designer setting about the user form |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Vba;
using System;
using System.IO;
public class VbaModuleCollectionMethodAddUserFormWithStringStringByteDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the VBA project
VbaProject vbaProject = workbook.VbaProject;
VbaModuleCollection vbaModules = vbaProject.Modules;
// Prepare parameters for AddUserForm
string formName = "UserForm1";
string formCode =
"Private Sub CommandButton1_Click()\n" +
"    MsgBox \"Hello from UserForm!\"\n" +
"End Sub";
// Create a simple designer storage (this would normally be the .frx binary data)
byte[] designerStorage = new byte[] { 0x00, 0x01, 0x02, 0x03 };
try
{
// Call AddUserForm with (String, String, Byte[]) parameters
int moduleIndex = vbaModules.AddUserForm(formName, formCode, designerStorage);
Console.WriteLine($"UserForm added successfully at index: {moduleIndex}");
Console.WriteLine($"Total VBA modules: {vbaModules.Count}");
// Save the workbook to see the VBA project changes
workbook.Save("AddUserFormDemo.xlsm", SaveFormat.Xlsm);
}
catch (Exception ex)
{
Console.WriteLine($"Error adding UserForm: {ex.Message}");
}
}
}
}
```
### See Also
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
