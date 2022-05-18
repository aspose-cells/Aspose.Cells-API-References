---
title: AbstractTextLoadOptions
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 60
url: /net/aspose.cells/abstracttextloadoptions/
---
## AbstractTextLoadOptions class

Common options for loading text values

```csharp
public class AbstractTextLoadOptions : LoadOptions
```

## Properties

| Name | Description |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter) { get; set; } | Indicates whether auto filtering the data when loading the files. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions) { get; set; } | Gets and sets the auto fitter options |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid) { get; set; } | Check whether data is valid in the template file. |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction) { get; set; } | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata) { get; set; } | Gets or sets a value that indicates whether the string in text file is converted to date data. |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata) { get; set; } | Gets or sets a value that indicates whether the string in text file is converted to numeric data. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo) { get; set; } | Gets or sets the system culture info at the time the file was loaded. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings) { get; } | Gets the default style settings for initializing styles of the workbook |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding) { get; set; } | Gets and sets the default encoding. Only applies for csv file. |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs) { get; set; } | Gets and sets individual font configs. Only works for the [`Workbook`](../workbook) which uses this [`LoadOptions`](../loadoptions) to load.&gt; |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted) { get; set; } | Ignore the data which are not printed if directly printing the file |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor) { get; set; } | Gets and sets the interrupt monitor. |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision) { get; set; } | Indicates whether not parsing a string value if the length is 15. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata) { get; set; } | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode) { get; set; } | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler) { get; set; } | The data handler for processing cells data when reading template file. |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter) { get; set; } | The filter to denote how to load data. |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat) { get; } | Gets the load format. |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy) { get; set; } | Indicates the strategy to apply style for parsed values when converting string value to number or datetime. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting) { get; set; } | Gets or sets the memory usage options. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen) { get; set; } | Indicates whether parsing the formula when reading the file. |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords) { get; set; } | Indicates whether parsing pivot cached records when loading the file. The default value is false. |
| [Password](../../aspose.cells/loadoptions/password) { get; set; } | Gets and set the password of the workbook. |
| [Region](../../aspose.cells/loadoptions/region) { get; set; } | Gets or sets the system regional settings based on CountryCode at the time the file was loaded. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback) { get; set; } | Gets or sets warning callback. |

## Methods

| Name | Description |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize)(PaperSizeType) | Sets the default print paper size from default printer's setting. |

### See Also

* class [LoadOptions](../loadoptions)
* namespace [Aspose.Cells](../../aspose.cells)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
