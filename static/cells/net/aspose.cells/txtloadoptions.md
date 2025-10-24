##Class TxtLoadOptions
Aspose.Cells.TxtLoadOptions class. Represents the options for loading text file
## TxtLoadOptions class
Represents the options for loading text file.
```csharp
public class TxtLoadOptions : AbstractTextLoadOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [TxtLoadOptions](txtloadoptions/#constructor)() | Creates the options for loading text file. |
| [TxtLoadOptions](txtloadoptions/#constructor_1)(LoadFormat) | Creates the options for loading text file. |
## Properties
| Name | Description |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Indicates whether auto filtering the data when loading the files.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Gets and sets the auto fitter options(Inherited from [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Check whether data is valid in the template file.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata/) { get; set; } | Gets or sets a value that indicates whether the string in text file is converted to date data. Default value is true.(Inherited from [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata/) { get; set; } | Gets or sets a value that indicates whether the string in text file is converted to numeric data. Default value is true.(Inherited from [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Gets or sets the regional settings used for the Workbook that will be loaded.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Gets the default style settings for initializing styles of the workbook(Inherited from [`LoadOptions`](../loadoptions/).) |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding/) { get; set; } | Gets and sets the default encoding. Only applies for csv file.(Inherited from [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [ExtendToNextSheet](../../aspose.cells/txtloadoptions/extendtonextsheet/) { get; set; } | Whether extends data to next sheet when the rows or columns of data exceed limit. Default is false. |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Gets and sets individual font configs. Only works for the [`Workbook`](../workbook/) which uses this [`LoadOptions`](../loadoptions/) to load.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [HasFormula](../../aspose.cells/txtloadoptions/hasformula/) { get; set; } | Indicates whether the text is formula if it starts with "=". |
| [HasTextQualifier](../../aspose.cells/txtloadoptions/hastextqualifier/) { get; set; } | Whether there is text qualifier for cell value. Default is true. |
| [HeaderColumnsCount](../../aspose.cells/txtloadoptions/headercolumnscount/) { get; set; } | The count of header columns to be repeated for extended sheets. |
| [HeaderRowsCount](../../aspose.cells/txtloadoptions/headerrowscount/) { get; set; } | The count of header rows to be repeated for extended sheets. |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignore the data which are not printed if directly printing the file(Inherited from [`LoadOptions`](../loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Indicates whether ignoring useless shapes.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Gets and sets the interrupt monitor.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [IsMultiEncoded](../../aspose.cells/txtloadoptions/ismultiencoded/) { get; set; } | True means that the file contains several encoding. |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision/) { get; set; } | Indicates whether not parsing a string value if the length is 15.(Inherited from [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | The data handler for processing cells data when reading template file.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | The filter to denote how to load data.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Gets the load format.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy/) { get; set; } | Indicates the strategy to apply style for parsed values when converting string value to number or datetime.(Inherited from [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [MaxColumnCount](../../aspose.cells/txtloadoptions/maxcolumncount/) { get; set; } | The maximum count of columns to be imported for one sheet. |
| [MaxRowCount](../../aspose.cells/txtloadoptions/maxrowcount/) { get; set; } | The maximum count of rows to be imported for one sheet. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Gets or sets the memory mode for loaded workbook.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Indicates whether parsing the formula when reading the file.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Indicates whether parsing pivot cached records when loading the file. The default value is false.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Gets and set the password of the workbook.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [PreferredParsers](../../aspose.cells/txtloadoptions/preferredparsers/) { get; set; } | Gets and sets preferred value parsers for loading text file. |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Gets or sets the regional settings used for the Workbook that will be loaded.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [Separator](../../aspose.cells/txtloadoptions/separator/) { get; set; } | Gets and sets character separator of text file. |
| [SeparatorString](../../aspose.cells/txtloadoptions/separatorstring/) { get; set; } | Gets and sets a string value as separator. |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) Sets the default standard font name(Inherited from [`LoadOptions`](../loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) Sets the default standard font size.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [TextQualifier](../../aspose.cells/txtloadoptions/textqualifier/) { get; set; } | Specifies the text qualifier for cell values. Default qualifier is '"'. |
| [TreatConsecutiveDelimitersAsOne](../../aspose.cells/txtloadoptions/treatconsecutivedelimitersasone/) { get; set; } | Whether consecutive delimiters should be treated as one. |
| [TreatQuotePrefixAsValue](../../aspose.cells/txtloadoptions/treatquoteprefixasvalue/) { get; set; } | Indicates whether the leading single quote sign should be taken as part of the value of one cell. Default is true. If it is false, the leading single quote will be removed from corresponding cell's value and [`QuotePrefix`](../style/quoteprefix/) will be set as true for the cell. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | Gets or sets warning callback.(Inherited from [`LoadOptions`](../loadoptions/).) |
## Methods
| Name | Description |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | Sets the default print paper size from default printer's setting.(Inherited from [`LoadOptions`](../loadoptions/).) |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Text;
public class TxtLoadOptionsDemo
{
public static void TxtLoadOptionsExample()
{
// Create an instance of TxtLoadOptions
TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
{
Separator = ',',
SeparatorString = ",",
IsMultiEncoded = false,
HasFormula = true,
HasTextQualifier = true,
TextQualifier = '\"',
TreatConsecutiveDelimitersAsOne = true,
TreatQuotePrefixAsValue = true,
ExtendToNextSheet = false,
HeaderRowsCount = 1,
HeaderColumnsCount = 1,
MaxRowCount = 1000,
MaxColumnCount = 50,
Encoding = Encoding.UTF8,
LoadStyleStrategy = TxtLoadStyleStrategy.BuiltIn,
ConvertNumericData = true,
ConvertDateTimeData = true,
KeepPrecision = true,
Password = "password",
ParsingFormulaOnOpen = true,
ParsingPivotCachedRecords = true,
LanguageCode = CountryCode.USA,
Region = CountryCode.USA,
CultureInfo = new System.Globalization.CultureInfo("en-US"),
StandardFont = "Arial",
StandardFontSize = 10.5,
InterruptMonitor = new InterruptMonitor(),
IgnoreNotPrinted = true,
CheckDataValid = true,
CheckExcelRestriction = true,
KeepUnparsedData = true,
LoadFilter = new LoadFilter(LoadDataFilterOptions.All),
LightCellsDataHandler = new LightCellsDataHandler(),
MemorySetting = MemorySetting.MemoryPreference,
WarningCallback = new WarningCallback(),
AutoFitterOptions = new AutoFitterOptions(),
AutoFilter = true,
FontConfigs = new IndividualFontConfigs(),
IgnoreUselessShapes = true,
PreservePaddingSpacesInFormula = true
};
// Load a CSV file with the specified options
Workbook workbook = new Workbook("TxtLoadOptionsExample_original.csv", loadOptions);
// Save the workbook to an Excel file
workbook.Save("TxtLoadOptionsExample.xlsx");
return;
}
}
// Dummy implementations for referenced classes/interfaces
public class InterruptMonitor : AbstractInterruptMonitor
{
public override bool IsInterruptionRequested => false;
}
public class WarningCallback : IWarningCallback
{
public void Warning(WarningInfo warningInfo)
{
Console.WriteLine(warningInfo.Description);
}
}
public class LightCellsDataHandler : Aspose.Cells.LightCellsDataHandler
{
public bool StartSheet(Worksheet sheet) => true;
public bool StartRow(int rowIndex) => true;
public bool ProcessRow(Row row) => true;
public bool StartCell(int columnIndex) => true;
public bool ProcessCell(Cell cell) => true;
}
}
```
### See Also
* class [AbstractTextLoadOptions](../abstracttextloadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
