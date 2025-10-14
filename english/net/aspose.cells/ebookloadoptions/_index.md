---
title: Class EbookLoadOptions
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.EbookLoadOptions class. Represents options when importing an ebook file
type: docs
url: /net/aspose.cells/ebookloadoptions/
---
## EbookLoadOptions class

Represents options when importing an ebook file.

```csharp
public class EbookLoadOptions : HtmlLoadOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [EbookLoadOptions](ebookloadoptions/#constructor)() | Creates an options of loading the ebook file. |
| [EbookLoadOptions](ebookloadoptions/#constructor_1)(LoadFormat) | Creates an options of loading the ebook file. |

## Properties

| Name | Description |
| --- | --- |
| [AttachedFilesDirectory](../../aspose.cells/htmlloadoptions/attachedfilesdirectory/) { get; set; } | (**Obsolete.**) The directory that the attached files will be saved to.(Inherited from [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Indicates whether auto filtering the data when loading the files.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [AutoFitColsAndRows](../../aspose.cells/htmlloadoptions/autofitcolsandrows/) { get; set; } | Indicates whether auto-fit columns and rows. The default value is false.(Inherited from [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Gets and sets the auto fitter options(Inherited from [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Check whether data is valid in the template file.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata/) { get; set; } | Gets or sets a value that indicates whether the string in text file is converted to date data. Default value is true.(Inherited from [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [ConvertFormulasData](../../aspose.cells/htmlloadoptions/convertformulasdata/) { get; set; } | (**Obsolete.**) if true, convert string to formula when string value starts with character '=',the default value is false.(Inherited from [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata/) { get; set; } | Gets or sets a value that indicates whether the string in text file is converted to numeric data. Default value is true.(Inherited from [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Gets or sets the regional settings used for the Workbook that will be loaded.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Gets the default style settings for initializing styles of the workbook(Inherited from [`LoadOptions`](../loadoptions/).) |
| [DeleteRedundantSpaces](../../aspose.cells/htmlloadoptions/deleteredundantspaces/) { get; set; } | Indicates whether delete redundant spaces when the text wraps lines using `<br>` tag. The default value is false.(Inherited from [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding/) { get; set; } | Gets and sets the default encoding. Only applies for csv file.(Inherited from [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Gets and sets individual font configs. Only works for the [`Workbook`](../workbook/) which uses this [`LoadOptions`](../loadoptions/) to load.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [HasFormula](../../aspose.cells/htmlloadoptions/hasformula/) { get; set; } | Indicates whether the text is formula if it starts with "=".(Inherited from [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignore the data which are not printed if directly printing the file(Inherited from [`LoadOptions`](../loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Indicates whether ignoring useless shapes.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Gets and sets the interrupt monitor.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision/) { get; set; } | Indicates whether not parsing a string value if the length is 15.(Inherited from [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | The data handler for processing cells data when reading template file.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | The filter to denote how to load data.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Gets the load format.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [LoadFormulas](../../aspose.cells/htmlloadoptions/loadformulas/) { get; set; } | Indicates whether importing formulas if the original html file contains formulas(Inherited from [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy/) { get; set; } | Indicates the strategy to apply style for parsed values when converting string value to number or datetime.(Inherited from [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Gets or sets the memory mode for loaded workbook.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Indicates whether parsing the formula when reading the file.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Indicates whether parsing pivot cached records when loading the file. The default value is false.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Gets and set the password of the workbook.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [ProgId](../../aspose.cells/htmlloadoptions/progid/) { get; } | Gets the program id of creating the file. Only for MHT files.(Inherited from [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Gets or sets the regional settings used for the Workbook that will be loaded.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) Sets the default standard font name(Inherited from [`LoadOptions`](../loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) Sets the default standard font size.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [StreamProvider](../../aspose.cells/htmlloadoptions/streamprovider/) { get; set; } | Gets or sets the StreamProviderImportHtmlFile for importing objects.(Inherited from [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [SupportDivTag](../../aspose.cells/htmlloadoptions/supportdivtag/) { get; set; } | Indicates whether support the layout of `<div>` tag when the html file contains it. The default value is false.(Inherited from [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [TableLoadOptions](../../aspose.cells/htmlloadoptions/tableloadoptions/) { get; } | Get the HtmlTableLoadOptionCollection instance(Inherited from [`HtmlLoadOptions`](../htmlloadoptions/).) |
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
    using System.IO;
    using System.Text;

    public class EbookLoadOptionsDemo
    {
        public static void EbookLoadOptionsExample()
        {
            // Create an instance of EbookLoadOptions
            EbookLoadOptions options = new EbookLoadOptions();

            // Setting properties
            options.AttachedFilesDirectory = "C:\\AttachedFiles";
            options.LoadFormulas = true;
            options.SupportDivTag = true;
            options.DeleteRedundantSpaces = true;
            options.AutoFitColsAndRows = true;
            options.ConvertFormulasData = true;
            options.HasFormula = true;
            options.Encoding = Encoding.UTF8;
            options.LoadStyleStrategy = TxtLoadStyleStrategy.None;
            options.ConvertNumericData = true;
            options.ConvertDateTimeData = true;
            options.KeepPrecision = true;
            options.Password = "password";
            options.ParsingFormulaOnOpen = true;
            options.ParsingPivotCachedRecords = true;
            options.LanguageCode = CountryCode.USA;
            options.Region = CountryCode.USA;
            options.CultureInfo = new System.Globalization.CultureInfo("en-US");
            options.StandardFont = "Arial";
            options.StandardFontSize = 12.0;
            options.InterruptMonitor = null; // Assuming no interrupt monitor is set
            options.IgnoreNotPrinted = true;
            options.CheckDataValid = true;
            options.CheckExcelRestriction = true;
            options.KeepUnparsedData = true;
            options.LoadFilter = new LoadFilter();
            options.LightCellsDataHandler = null; // Assuming no light cells data handler is set
            options.MemorySetting = MemorySetting.Normal;
            options.WarningCallback = null; // Assuming no warning callback is set
            options.AutoFitterOptions = new AutoFitterOptions();
            options.AutoFilter = true;
            options.FontConfigs = new IndividualFontConfigs();
            options.IgnoreUselessShapes = true;
            options.PreservePaddingSpacesInFormula = true;

            // Load an ebook file into a Workbook using the specified options
            Workbook workbook = new Workbook("EbookLoadOptionsExample_original.ebook", options);

            // Save the workbook to an Excel file
            workbook.Save("EbookLoadOptionsExample.xlsx");

            return;
        }
    }
}
```

### See Also

* class [HtmlLoadOptions](../htmlloadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


