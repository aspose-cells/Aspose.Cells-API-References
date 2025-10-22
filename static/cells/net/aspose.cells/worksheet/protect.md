##Worksheet.Protect
Worksheet method. Protects worksheet
## Protect(ProtectionType) {#protect}
Protects worksheet.
```csharp
public void Protect(ProtectionType type)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | ProtectionType | Protection type. |
### Remarks
This method protects worksheet without password. It can protect worksheet in all versions of Excel file.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodProtectWithProtectionTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet sheet = workbook.Worksheets[0];
// Protect the worksheet with Objects protection type
sheet.Protect(ProtectionType.Objects);
// Save the workbook
workbook.Save("ProtectedWorksheet.xlsx");
}
}
}
```
### See Also
* enum [ProtectionType](../../protectiontype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Protect(ProtectionType, string, string) {#protect_1}
Protects worksheet.
```csharp
public void Protect(ProtectionType type, string password, string oldPassword)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | ProtectionType | Protection type. |
| password | String | Password. |
| oldPassword | String | If the worksheet is already protected by a password, please supply the old password. Otherwise, you can set a null value or blank string to this parameter. |
### Remarks
This method can protect worksheet in all versions of Excel file.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodProtectWithProtectionTypeStringStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Protect the worksheet with password and allow all protection types
worksheet.Protect(ProtectionType.All, "password123", null);
// Save the workbook
workbook.Save("ProtectedWorksheet.xlsx");
}
}
}
```
### See Also
* enum [ProtectionType](../../protectiontype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
