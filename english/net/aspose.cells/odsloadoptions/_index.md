---
title: OdsLoadOptions
second_title: Aspose.Cells for .NET API Reference
description: Represents the options of loading ods file.
type: docs
weight: 4360
url: /net/aspose.cells/odsloadoptions/
---
## OdsLoadOptions class

Represents the options of loading ods file.

```csharp
public class OdsLoadOptions : LoadOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [OdsLoadOptions](odsloadoptions#constructor)() | Represents the options of loading ods file. |
| [OdsLoadOptions](odsloadoptions#constructor_1)(LoadFormat) | Represents the options of loading ods file. |

## Properties

| Name | Description |
| --- | --- |
| [ApplyExcelDefaultStyleToHyperlink](../../aspose.cells/odsloadoptions/applyexceldefaultstyletohyperlink) { get; set; } | Indicates whether applying the default style of the Excel to hyperlink. |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter) { get; set; } | Indicates whether auto filtering the data when loading the files.(Inherited from [`LoadOptions`](../loadoptions).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions) { get; set; } | Gets and sets the auto fitter options(Inherited from [`LoadOptions`](../loadoptions).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid) { get; set; } | Check whether data is valid in the template file.(Inherited from [`LoadOptions`](../loadoptions).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction) { get; set; } | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.(Inherited from [`LoadOptions`](../loadoptions).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo) { get; set; } | Gets or sets the system culture info at the time the file was loaded.(Inherited from [`LoadOptions`](../loadoptions).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings) { get; } | Gets the default style settings for initializing styles of the workbook(Inherited from [`LoadOptions`](../loadoptions).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs) { get; set; } | Gets and sets individual font configs. Only works for the [`Workbook`](../workbook) which uses this [`LoadOptions`](../loadoptions) to load.&gt;(Inherited from [`LoadOptions`](../loadoptions).) |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted) { get; set; } | Ignore the data which are not printed if directly printing the file(Inherited from [`LoadOptions`](../loadoptions).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor) { get; set; } | Gets and sets the interrupt monitor.(Inherited from [`LoadOptions`](../loadoptions).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata) { get; set; } | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true.(Inherited from [`LoadOptions`](../loadoptions).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode) { get; set; } | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file.(Inherited from [`LoadOptions`](../loadoptions).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler) { get; set; } | The data handler for processing cells data when reading template file.(Inherited from [`LoadOptions`](../loadoptions).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter) { get; set; } | The filter to denote how to load data.(Inherited from [`LoadOptions`](../loadoptions).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat) { get; } | Gets the load format.(Inherited from [`LoadOptions`](../loadoptions).) |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting) { get; set; } | Gets or sets the memory usage options.(Inherited from [`LoadOptions`](../loadoptions).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen) { get; set; } | Indicates whether parsing the formula when reading the file.(Inherited from [`LoadOptions`](../loadoptions).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords) { get; set; } | Indicates whether parsing pivot cached records when loading the file. The default value is false.(Inherited from [`LoadOptions`](../loadoptions).) |
| [Password](../../aspose.cells/loadoptions/password) { get; set; } | Gets and set the password of the workbook.(Inherited from [`LoadOptions`](../loadoptions).) |
| [RefreshPivotTables](../../aspose.cells/odsloadoptions/refreshpivottables) { get; set; } | Indicates whether refresh pivot tables when loading file. |
| [Region](../../aspose.cells/loadoptions/region) { get; set; } | Gets or sets the system regional settings based on CountryCode at the time the file was loaded.(Inherited from [`LoadOptions`](../loadoptions).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont) { get; set; } | (**Obsolete.**) Sets the default standard font name(Inherited from [`LoadOptions`](../loadoptions).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize) { get; set; } | (**Obsolete.**) Sets the default standard font size.(Inherited from [`LoadOptions`](../loadoptions).) |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback) { get; set; } | Gets or sets warning callback.(Inherited from [`LoadOptions`](../loadoptions).) |

## Methods

| Name | Description |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize)(PaperSizeType) | Sets the default print paper size from default printer's setting.(Inherited from [`LoadOptions`](../loadoptions).) |

### See Also

* class [LoadOptions](../loadoptions)
* namespace [Aspose.Cells](../../aspose.cells)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
