##Enum DefaultEditLanguage
Aspose.Cells.DefaultEditLanguage enum. Represents the default edit language
## DefaultEditLanguage enumeration
Represents the default edit language.
```csharp
public enum DefaultEditLanguage
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Auto | `0` | Represents auto detecting edit language according to the text itself. |
| English | `1` | Represents English language. |
| CJK | `2` | Represents Chinese, Japanese, Korean language. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class DefaultEditLanguageDemo
{
public static void DefaultEditLanguageExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create AutoFitterOptions and set DefaultEditLanguage
AutoFitterOptions autoFitterOptions = new AutoFitterOptions();
autoFitterOptions.DefaultEditLanguage = DefaultEditLanguage.CJK;
// Apply auto fit rows with the specified options
worksheet.AutoFitRows(autoFitterOptions);
// Save the workbook
workbook.Save("DefaultEditLanguageExample.xlsx");
workbook.Save("DefaultEditLanguageExample.pdf");
// Output the set DefaultEditLanguage to the console
Console.WriteLine("Default Edit Language set to: " + autoFitterOptions.DefaultEditLanguage);
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
