---
title: HtmlLoadOptions Class 
linktitle: HtmlLoadOptions
second_title: Aspose.Cells for Go via C++ API Reference
description: 'HtmlLoadOptions class. Encapsulates the object that represents htmlloadoptions in Go.'
type: docs
weight: 200
url: /go-cpp/htmlloadoptions/
---

## HtmlLoadOptions class

Represents options when importing a html file.

```go

type HtmlLoadOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
|[NewHtmlLoadOptions](./newhtmlloadoptions/) | Creates an options of loading the file. | 
|[NewHtmlLoadOptions_LoadFormat](./newhtmlloadoptions_loadformat/) | Creates an options of loading the file. | 
|[NewHtmlLoadOptions_AbstractTextLoadOptions](./newhtmlloadoptions_abstracttextloadoptions/) | Constructs from a parent object. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetLoadFormulas](./getloadformulas/) | Indicates whether importing formulas if the original html file contains formulas | 
|[SetLoadFormulas](./setloadformulas/) | Indicates whether importing formulas if the original html file contains formulas | 
|[GetSupportDivTag](./getsupportdivtag/) | Indicates whether support the layout of <c>&lt;div&gt;</c> tag when the html file contains it.The default value is false. | 
|[SetSupportDivTag](./setsupportdivtag/) | Indicates whether support the layout of <c>&lt;div&gt;</c> tag when the html file contains it.The default value is false. | 
|[GetDeleteRedundantSpaces](./getdeleteredundantspaces/) | Indicates whether delete redundant spaces when the text wraps lines using <c>&lt;br&gt;</c> tag.The default value is false. | 
|[SetDeleteRedundantSpaces](./setdeleteredundantspaces/) | Indicates whether delete redundant spaces when the text wraps lines using <c>&lt;br&gt;</c> tag.The default value is false. | 
|[GetAutoFitColsAndRows](./getautofitcolsandrows/) | Indicates whether auto-fit columns and rows. The default value is false. | 
|[SetAutoFitColsAndRows](./setautofitcolsandrows/) | Indicates whether auto-fit columns and rows. The default value is false. | 
|[GetHasFormula](./gethasformula/) | Indicates whether the text is formula if it starts with "=". | 
|[SetHasFormula](./sethasformula/) | Indicates whether the text is formula if it starts with "=". | 
|[GetProgId](./getprogid/) | Gets the program id of creating the file.Only for MHT files. | 
|[GetTableLoadOptions](./gettableloadoptions/) | Get the HtmlTableLoadOptionCollection instance | 
|[GetEncoding](./getencoding/) | Gets and sets the default encoding. Only applies for csv file. | 
|[SetEncoding](./setencoding/) | Gets and sets the default encoding. Only applies for csv file. | 
|[GetLoadStyleStrategy](./getloadstylestrategy/) | Indicates the strategy to apply style for parsed values when converting string value to number or datetime. | 
|[SetLoadStyleStrategy](./setloadstylestrategy/) | Indicates the strategy to apply style for parsed values when converting string value to number or datetime. | 
|[GetConvertNumericData](./getconvertnumericdata/) | Gets or sets a value that indicates whether the string in text file is converted to numeric data.Default value is true. | 
|[SetConvertNumericData](./setconvertnumericdata/) | Gets or sets a value that indicates whether the string in text file is converted to numeric data.Default value is true. | 
|[GetConvertDateTimeData](./getconvertdatetimedata/) | Gets or sets a value that indicates whether the string in text file is converted to date data.Default value is true. | 
|[SetConvertDateTimeData](./setconvertdatetimedata/) | Gets or sets a value that indicates whether the string in text file is converted to date data.Default value is true. | 
|[GetKeepPrecision](./getkeepprecision/) | Indicates whether not parsing a string value if the length is 15. | 
|[SetKeepPrecision](./setkeepprecision/) | Indicates whether not parsing a string value if the length is 15. | 
|[GetLoadFormat](./getloadformat/) | Gets the load format. | 
|[GetPassword](./getpassword/) | Gets and set the password of the workbook. | 
|[SetPassword](./setpassword/) | Gets and set the password of the workbook. | 
|[GetParsingFormulaOnOpen](./getparsingformulaonopen/) | Indicates whether parsing the formula when reading the file. | 
|[SetParsingFormulaOnOpen](./setparsingformulaonopen/) | Indicates whether parsing the formula when reading the file. | 
|[GetParsingPivotCachedRecords](./getparsingpivotcachedrecords/) | Indicates whether parsing pivot cached records when loading the file.The default value is false. | 
|[SetParsingPivotCachedRecords](./setparsingpivotcachedrecords/) | Indicates whether parsing pivot cached records when loading the file.The default value is false. | 
|[SetPaperSize](./setpapersize/) | Sets the default print paper size from default printer's setting. | 
|[GetLanguageCode](./getlanguagecode/) | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. | 
|[SetLanguageCode](./setlanguagecode/) | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. | 
|[GetRegion](./getregion/) | Gets or sets the regional settings used for the Workbook that will be loaded. | 
|[SetRegion](./setregion/) | Gets or sets the regional settings used for the Workbook that will be loaded. | 
|[GetDefaultStyleSettings](./getdefaultstylesettings/) | Gets the default style settings for initializing styles of the workbook | 
|[GetInterruptMonitor](./getinterruptmonitor/) | Gets and sets the interrupt monitor. | 
|[SetInterruptMonitor](./setinterruptmonitor/) | Gets and sets the interrupt monitor. | 
|[GetIgnoreNotPrinted](./getignorenotprinted/) | Ignore the data which are not printed if directly printing the file | 
|[SetIgnoreNotPrinted](./setignorenotprinted/) | Ignore the data which are not printed if directly printing the file | 
|[GetCheckDataValid](./getcheckdatavalid/) | Check whether data is valid in the template file. | 
|[SetCheckDataValid](./setcheckdatavalid/) | Check whether data is valid in the template file. | 
|[GetCheckExcelRestriction](./getcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects.For example, excel does not allow inputting string value longer than 32K.When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception.If this property is false, we will accept your input string value as the cell's value so that lateryou can output the complete string value for other file formats such as CSV.However, if you have set such kind of value that is invalid for excel file format,you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. | 
|[SetCheckExcelRestriction](./setcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects.For example, excel does not allow inputting string value longer than 32K.When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception.If this property is false, we will accept your input string value as the cell's value so that lateryou can output the complete string value for other file formats such as CSV.However, if you have set such kind of value that is invalid for excel file format,you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. | 
|[GetKeepUnparsedData](./getkeepunparseddata/) | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. | 
|[SetKeepUnparsedData](./setkeepunparseddata/) | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. | 
|[GetLoadFilter](./getloadfilter/) | The filter to denote how to load data. | 
|[SetLoadFilter](./setloadfilter/) | The filter to denote how to load data. | 
|[GetMemorySetting](./getmemorysetting/) | Gets or sets the memory mode for loaded workbook. | 
|[SetMemorySetting](./setmemorysetting/) | Gets or sets the memory mode for loaded workbook. | 
|[GetAutoFitterOptions](./getautofitteroptions/) | Gets and sets the auto fitter options | 
|[SetAutoFitterOptions](./setautofitteroptions/) | Gets and sets the auto fitter options | 
|[GetAutoFilter](./getautofilter/) | Indicates whether auto filtering the data when loading the files. | 
|[SetAutoFilter](./setautofilter/) | Indicates whether auto filtering the data when loading the files. | 
|[GetFontConfigs](./getfontconfigs/) | Gets and sets individual font configs.Only works for the Workbook which uses this LoadOptions to load. | 
|[SetFontConfigs](./setfontconfigs/) | Gets and sets individual font configs.Only works for the Workbook which uses this LoadOptions to load. | 
|[GetIgnoreUselessShapes](./getignoreuselessshapes/) | Indicates whether ignoring useless shapes. | 
|[SetIgnoreUselessShapes](./setignoreuselessshapes/) | Indicates whether ignoring useless shapes. | 
|[GetPreservePaddingSpacesInFormula](./getpreservepaddingspacesinformula/) | Indicates whether preserve those spaces and line breaks that are padded between formula tokenswhile getting and setting formulas.Default value is false. | 
|[SetPreservePaddingSpacesInFormula](./setpreservepaddingspacesinformula/) | Indicates whether preserve those spaces and line breaks that are padded between formula tokenswhile getting and setting formulas.Default value is false. | 
