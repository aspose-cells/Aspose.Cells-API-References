##WorkbookSettings.Compliance
WorkbookSettings property. Specifies the OOXML version for the output document. The default value is Ecma376_2006
## WorkbookSettings.Compliance property
Specifies the OOXML version for the output document. The default value is Ecma376_2006.
```csharp
public OoxmlCompliance Compliance { get; set; }
```
### Remarks
Only for .xlsx files.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyComplianceDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
WorkbookSettings settings = workbook.Settings;
// Set compliance to strict mode
settings.Compliance = OoxmlCompliance.Iso29500_2008_Strict;
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Strict Compliance Demo");
workbook.Save("WorkbookComplianceDemo.xlsx");
}
}
}
```
### See Also
* enum [OoxmlCompliance](../../ooxmlcompliance/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
