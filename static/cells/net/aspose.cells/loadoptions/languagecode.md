##LoadOptions.LanguageCode
LoadOptions property. Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file
## LoadOptions.LanguageCode property
Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file.
```csharp
public CountryCode LanguageCode { get; set; }
```
### Examples
```csharp
using System;
using System.Globalization;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class LoadOptionsPropertyLanguageCodeDemo
{
public static void Run()
{
// Create an instance of LoadOptions
LoadOptions loadOptions = new LoadOptions();
// Set LanguageCode property
loadOptions.LanguageCode = CountryCode.USA;
// Load a workbook with the specified LoadOptions
Workbook workbook = new Workbook("sample.xlsx", loadOptions);
// Access worksheet and modify content
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Language Code Demo");
// Save the modified workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* enum [CountryCode](../../countrycode/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
