##OdsSaveOptions.IsStrictSchema11
OdsSaveOptions property. Indicates whether the ods file should be saved as ODF format version 1.1. Default is false
## OdsSaveOptions.IsStrictSchema11 property
Indicates whether the ods file should be saved as ODF format version 1.1. Default is false.
```csharp
[Obsolete("Use OdsSaveOptions.OdfStrictVersion property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsStrictSchema11 { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use OdsSaveOptions.OdfStrictVersion property. This method will be removed 12 months later since February 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class OdsSaveOptionsPropertyIsStrictSchema11Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample ODS with strict schema");
OdsSaveOptions saveOptions = new OdsSaveOptions();
saveOptions.IsStrictSchema11 = true;
workbook.Save("StrictSchema11Example.ods", saveOptions);
}
}
}
```
### See Also
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
