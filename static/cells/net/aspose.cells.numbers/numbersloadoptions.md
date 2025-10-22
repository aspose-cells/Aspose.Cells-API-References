##Class NumbersLoadOptions
Aspose.Cells.Numbers.NumbersLoadOptions class. Represents the options of loading Apple Numbers files
## NumbersLoadOptions class
Represents the options of loading Apple Numbers files.
```csharp
public class NumbersLoadOptions : LoadOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [NumbersLoadOptions](numbersloadoptions/)() | Constructor. |
## Properties
| Name | Description |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Indicates whether auto filtering the data when loading the files.(Inherited from [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Gets and sets the auto fitter options(Inherited from [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Check whether data is valid in the template file.(Inherited from [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.(Inherited from [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Gets or sets the regional settings used for the Workbook that will be loaded.(Inherited from [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Gets the default style settings for initializing styles of the workbook(Inherited from [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Gets and sets individual font configs. Only works for the [`Workbook`](../../aspose.cells/workbook/) which uses this [`LoadOptions`](../../aspose.cells/loadoptions/) to load.(Inherited from [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignore the data which are not printed if directly printing the file(Inherited from [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Indicates whether ignoring useless shapes.(Inherited from [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Gets and sets the interrupt monitor.(Inherited from [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true.(Inherited from [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file.(Inherited from [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | The data handler for processing cells data when reading template file.(Inherited from [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | The filter to denote how to load data.(Inherited from [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Gets the load format.(Inherited from [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LoadTableType](../../aspose.cells.numbers/numbersloadoptions/loadtabletype/) { get; set; } | Gets and sets the type of loading multiple tables in one worksheet. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Gets or sets the memory mode for loaded workbook.(Inherited from [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Indicates whether parsing the formula when reading the file.(Inherited from [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Indicates whether parsing pivot cached records when loading the file. The default value is false.(Inherited from [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Gets and set the password of the workbook.(Inherited from [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false.(Inherited from [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Gets or sets the regional settings used for the Workbook that will be loaded.(Inherited from [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) Sets the default standard font name(Inherited from [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) Sets the default standard font size.(Inherited from [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | Gets or sets warning callback.(Inherited from [`LoadOptions`](../../aspose.cells/loadoptions/).) |
## Methods
| Name | Description |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | Sets the default print paper size from default printer's setting.(Inherited from [`LoadOptions`](../../aspose.cells/loadoptions/).) |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Numbers;
using System;
using System.Globalization;
public class NumbersLoadOptionsDemo
{
public static void NumbersLoadOptionsExample()
{
// Create an instance of NumbersLoadOptions
NumbersLoadOptions loadOptions = new NumbersLoadOptions
{
// Setting properties
LoadTableType = LoadNumbersTableType.OneTablePerSheet,
Password = "password123",
ParsingFormulaOnOpen = true,
ParsingPivotCachedRecords = false,
LanguageCode = CountryCode.USA,
Region = CountryCode.USA,
CultureInfo = new CultureInfo("en-US"),
StandardFont = "Arial",
StandardFontSize = 10.5,
IgnoreNotPrinted = true,
CheckDataValid = true,
CheckExcelRestriction = true,
KeepUnparsedData = true,
LoadFilter = new LoadFilter(LoadDataFilterOptions.All),
LightCellsDataHandler = new CustomLightCellsDataHandler(),
MemorySetting = MemorySetting.MemoryPreference,
WarningCallback = new CustomWarningCallback(),
AutoFitterOptions = new AutoFitterOptions { AutoFitMergedCells = true },
AutoFilter = true,
FontConfigs = new IndividualFontConfigs(),
IgnoreUselessShapes = true,
PreservePaddingSpacesInFormula = false
};
// Load a Numbers file with the specified load options
Workbook workbook = new Workbook("NumbersLoadOptionsExample_original.numbers", loadOptions);
// Save the workbook in XLSX format
workbook.Save("NumbersLoadOptionsExample.xlsx");
}
}
// Custom implementation of LightCellsDataHandler
public class CustomLightCellsDataHandler : LightCellsDataHandler
{
public bool ProcessCell(Cell cell)
{
return true;
}
public bool ProcessRow(Row row)
{
return true;
}
public bool StartCell(int columnIndex)
{
return true;
}
public bool StartRow(int rowIndex)
{
return true;
}
public bool StartSheet(Worksheet sheet)
{
return true;
}
}
// Custom implementation of IWarningCallback
public class CustomWarningCallback : IWarningCallback
{
public void Warning(WarningInfo warningInfo)
{
Console.WriteLine($"Warning: {warningInfo.Description}");
}
}
}
```
### See Also
* class [LoadOptions](../../aspose.cells/loadoptions/)
* namespace [Aspose.Cells.Numbers](../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../)
