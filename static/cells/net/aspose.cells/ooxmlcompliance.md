##Enum OoxmlCompliance
Aspose.Cells.OoxmlCompliance enum. Allows to specify which OOXML specification will be used when saving in the Xlsx format
## OoxmlCompliance enumeration
Allows to specify which OOXML specification will be used when saving in the Xlsx format.
```csharp
public enum OoxmlCompliance
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Ecma376_2006 | `0` | ECMA-376 1st Edition, 2006. |
| Iso29500_2008_Strict | `1` | ISO/IEC 29500:2008 Strict compliance level. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class OoxmlComplianceDemo
{
public static void OoxmlComplianceExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access workbook settings
WorkbookSettings settings = workbook.Settings;
// Set the OOXML compliance level to ISO/IEC 29500:2008 Strict
settings.Compliance = OoxmlCompliance.Iso29500_2008_Strict;
// Add some data to the worksheet
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells[0, 0].PutValue("Hello, World!");
// Save the workbook with the specified OOXML compliance level
workbook.Save("OoxmlComplianceExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
