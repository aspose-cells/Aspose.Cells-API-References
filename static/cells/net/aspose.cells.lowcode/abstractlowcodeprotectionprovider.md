##Class AbstractLowCodeProtectionProvider
Aspose.Cells.LowCode.AbstractLowCodeProtectionProvider class. Implementation to provide protection settings
## AbstractLowCodeProtectionProvider class
Implementation to provide protection settings
```csharp
public class AbstractLowCodeProtectionProvider
```
## Constructors
| Name | Description |
| --- | --- |
| [AbstractLowCodeProtectionProvider](abstractlowcodeprotectionprovider/)() | The default constructor. |
## Methods
| Name | Description |
| --- | --- |
| virtual [GetOpenPassword](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getopenpassword/)() | Gets the password to open spread sheet file. |
| virtual [GetWorkbookPassword](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworkbookpassword/)() | Gets the password to protect the workbook with specified protection type. |
| virtual [GetWorkbookProtectionType](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworkbookprotectiontype/)() | Gets the protection type to protect the workbook. |
| virtual [GetWorksheetPassword](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworksheetpassword/)(string) | Gets the password to protect the specified worksheet. |
| virtual [GetWorksheetProtectionType](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworksheetprotectiontype/)(string) | Gets the protection type to protect the specified worksheet. |
| virtual [GetWritePassword](../../aspose.cells.lowcode/abstractlowcodeprotectionprovider/getwritepassword/)() | Gets the password to modify spread sheet file. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class LowCodeClassAbstractLowCodeProtectionProviderDemo
{
public static void Run()
{
// Create a new workbook and add test worksheets
Workbook workbook = new Workbook();
workbook.Worksheets.Add("SalesData");
workbook.Worksheets.Add("AuditReport");
// Create custom protection provider instance
var protectionProvider = new CustomProtectionProvider();
// Apply workbook protection
workbook.Protect(
protectionProvider.GetWorkbookProtectionType(),
protectionProvider.GetWorkbookPassword()
);
// Apply protection to all worksheets
foreach (Worksheet worksheet in workbook.Worksheets)
{
worksheet.Protect(
protectionProvider.GetWorksheetProtectionType(worksheet.Name),
null,  // Add null for oldPassword parameter
protectionProvider.GetWorksheetPassword(worksheet.Name)
);
}
// Set file access passwords
workbook.Settings.Password = protectionProvider.GetOpenPassword();
workbook.Settings.WriteProtection.Password = protectionProvider.GetWritePassword();
// Save protected workbook
workbook.Save("AbstractLowCodeProtectionProviderDemo.xlsx");
}
}
public class CustomProtectionProvider : AbstractLowCodeProtectionProvider
{
public override string GetOpenPassword() => "SecureOpen123";
public override string GetWritePassword() => "EditPermission456";
public override string GetWorkbookPassword() => "WorkbookLock789";
public override ProtectionType GetWorkbookProtectionType() =>
ProtectionType.Windows;  // Prevent window structure changes
public override string GetWorksheetPassword(string sheetName) =>
$"SheetLock_{sheetName}";  // Dynamic password per sheet
public override ProtectionType GetWorksheetProtectionType(string sheetName) =>
ProtectionType.Contents;  // Protect cell contents
}
}
```
### See Also
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)
