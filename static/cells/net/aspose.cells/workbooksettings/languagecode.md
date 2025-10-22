##WorkbookSettings.LanguageCode
WorkbookSettings property. Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file
## WorkbookSettings.LanguageCode property
Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file.
```csharp
public CountryCode LanguageCode { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyLanguageCodeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access workbook settings
WorkbookSettings settings = workbook.Settings;
// Set language code to German (Germany)
settings.LanguageCode = CountryCode.Germany;
// Display the current language code
Console.WriteLine("Current Language Code: " + settings.LanguageCode);
// Change language code to French (France)
settings.LanguageCode = CountryCode.France;
Console.WriteLine("Updated Language Code: " + settings.LanguageCode);
// Save the workbook
workbook.Save("WorkbookSettings_LanguageCodeDemo.xlsx");
}
}
}
```
### See Also
* enum [CountryCode](../../countrycode/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
