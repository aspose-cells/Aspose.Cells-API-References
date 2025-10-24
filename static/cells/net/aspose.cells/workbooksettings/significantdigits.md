##WorkbookSettings.SignificantDigits
WorkbookSettings property. Gets and sets the number of significant digits. The default value is SignificantDigits
## WorkbookSettings.SignificantDigits property
Gets and sets the number of significant digits. The default value is [`SignificantDigits`](../../cellshelper/significantdigits/).
```csharp
[Obsolete("Use SignificantDigitsType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int SignificantDigits { get; set; }
```
### Remarks
Only could be 15 or 17 now. NOTE: This member is now obsolete. Instead, please use [`SignificantDigitsType`](../significantdigitstype/). This property will be removed 12 months later since June 2025. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using System.Globalization;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertySignificantDigitsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample numeric data to demonstrate significant digits
sheet.Cells["A1"].PutValue(123.4567890123456789);
sheet.Cells["A2"].PutValue(0.000000000123456789);
// Access workbook settings
WorkbookSettings settings = workbook.Settings;
// Set significant digits to 15 (maximum precision for double)
settings.SignificantDigits = 15;
// Save the workbook to show the effect of significant digits
workbook.Save("SignificantDigitsDemo.xlsx");
Console.WriteLine("Workbook saved with SignificantDigits set to 15.");
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
