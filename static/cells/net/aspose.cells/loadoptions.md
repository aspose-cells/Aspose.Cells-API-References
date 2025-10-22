##Class LoadOptions
Aspose.Cells.LoadOptions class. Represents the options of loading the file
## LoadOptions class
Represents the options of loading the file.
```csharp
public class LoadOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [LoadOptions](loadoptions/#constructor)() | Creates an options of loading the file. |
| [LoadOptions](loadoptions/#constructor_1)(LoadFormat) | Creates an options of loading the file. |
## Properties
| Name | Description |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Indicates whether auto filtering the data when loading the files. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Gets and sets the auto fitter options |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Check whether data is valid in the template file. |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Gets or sets the regional settings used for the Workbook that will be loaded. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Gets the default style settings for initializing styles of the workbook |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Gets and sets individual font configs. Only works for the [`Workbook`](../workbook/) which uses this `LoadOptions` to load. |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignore the data which are not printed if directly printing the file |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Indicates whether ignoring useless shapes. |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Gets and sets the interrupt monitor. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | The data handler for processing cells data when reading template file. |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | The filter to denote how to load data. |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Gets the load format. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Gets or sets the memory mode for loaded workbook. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Indicates whether parsing the formula when reading the file. |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Indicates whether parsing pivot cached records when loading the file. The default value is false. |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Gets and set the password of the workbook. |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Gets or sets the regional settings used for the Workbook that will be loaded. |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) Sets the default standard font name |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) Sets the default standard font size. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | Gets or sets warning callback. |
## Methods
| Name | Description |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | Sets the default print paper size from default printer's setting. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Globalization;
public class LoadOptionsDemo
{
public static void LoadOptionsExample()
{
// Create an instance of LoadOptions
LoadOptions loadOptions = new LoadOptions();
// Setting properties
loadOptions.Password = "password123";
loadOptions.ParsingFormulaOnOpen = true;
loadOptions.ParsingPivotCachedRecords = false;
loadOptions.LanguageCode = CountryCode.USA;
loadOptions.Region = CountryCode.USA;
loadOptions.CultureInfo = new CultureInfo("en-US");
loadOptions.IgnoreNotPrinted = true;
loadOptions.CheckDataValid = true;
loadOptions.CheckExcelRestriction = false;
loadOptions.KeepUnparsedData = true;
loadOptions.MemorySetting = MemorySetting.MemoryPreference;
loadOptions.AutoFitterOptions = new AutoFitterOptions { AutoFitMergedCells = true };
loadOptions.AutoFilter = true;
loadOptions.IgnoreUselessShapes = true;
loadOptions.PreservePaddingSpacesInFormula = false;
// Load a workbook with the specified LoadOptions
Workbook workbook = new Workbook("LoadOptionsExample_original.xlsx", loadOptions);
// Perform operations on the workbook
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Hello, World!");
// Save the workbook
workbook.Save("LoadOptionsExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
