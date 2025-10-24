##Worksheet.Unprotect
Worksheet method. Unprotects worksheet
## Unprotect() {#unprotect}
Unprotects worksheet.
```csharp
public void Unprotect()
```
### Remarks
This method unprotects worksheet which is protected without password.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class WorksheetMethodUnprotectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Protect the worksheet with a password
worksheet.Protect(ProtectionType.All, "password123", null);
Console.WriteLine("Worksheet is protected: " + worksheet.IsProtected);
try
{
// Unprotect the worksheet without password (should fail)
worksheet.Unprotect();
Console.WriteLine("Worksheet unprotected without password: " + !worksheet.IsProtected);
}
catch (Exception ex)
{
Console.WriteLine("Error when trying to unprotect without password: " + ex.Message);
}
try
{
// Unprotect the worksheet with wrong password (should fail)
worksheet.Unprotect("wrongpassword");
Console.WriteLine("Worksheet unprotected with wrong password: " + !worksheet.IsProtected);
}
catch (Exception ex)
{
Console.WriteLine("Error when trying to unprotect with wrong password: " + ex.Message);
}
try
{
// Unprotect the worksheet with correct password
worksheet.Unprotect("password123");
Console.WriteLine("Worksheet successfully unprotected: " + !worksheet.IsProtected);
}
catch (Exception ex)
{
Console.WriteLine("Error when trying to unprotect: " + ex.Message);
}
// Save the result
workbook.Save("WorksheetMethodUnprotectDemo.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Unprotect(string) {#unprotect_1}
Unprotects worksheet.
```csharp
public void Unprotect(string password)
```
| Parameter | Type | Description |
| --- | --- | --- |
| password | String | Password |
### Remarks
If the worksheet is protected without a password, you can set a null value or blank string to password parameter.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodUnprotectWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Protect the worksheet with password and default protection type
worksheet.Protect(ProtectionType.All, "test", null);
// Unprotect the worksheet with password
worksheet.Unprotect("test");
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
