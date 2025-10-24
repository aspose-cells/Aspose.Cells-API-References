##WorkbookSettings.DefaultStyleSettings
WorkbookSettings property. Gets the settings for default values of stylerelated properties for this workbook
## WorkbookSettings.DefaultStyleSettings property
Gets the settings for default values of style-related properties for this workbook.
```csharp
public DefaultStyleSettings DefaultStyleSettings { get; }
```
### Examples
```csharp
using System;
using System.Globalization;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyDefaultStyleSettingsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the default style settings
DefaultStyleSettings styleSettings = workbook.Settings.DefaultStyleSettings;
// Set built-in number format preference
styleSettings.BuiltInPreference = true;
// Set culture for number formatting
workbook.Settings.CultureInfo = new CultureInfo("en-US");
// Access cells and apply formatting
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set values and styles
cells["A1"].PutValue(1234.56);
cells["A1"].GetStyle().Number = 4; // Currency format
cells["B1"].PutValue(0.456);
cells["B1"].GetStyle().Number = 2; // Percentage format
cells["C1"].PutValue(DateTime.Now);
cells["C1"].GetStyle().Number = 22; // Short date format
// Save the workbook
workbook.Save("DefaultStyleSettingsDemo.xlsx");
}
}
}
```
### See Also
* class [DefaultStyleSettings](../../defaultstylesettings/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
