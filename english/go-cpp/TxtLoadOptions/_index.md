---
title: TxtLoadOptions Class 
linktitle: TxtLoadOptions
second_title: Aspose.Cells for Go via C++ API Reference
description: 'TxtLoadOptions class. Encapsulates the object that represents txtloadoptions in Go.'
type: docs
weight: 200
url: /go-cpp/txtloadoptions/
---

## TxtLoadOptions class

Represents the options for loading text file.

```go

type TxtLoadOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
|[NewTxtLoadOptions](./newtxtloadoptions/) | Creates the options for loading text file. | 
|[NewTxtLoadOptions_LoadFormat](./newtxtloadoptions_loadformat/) | Creates the options for loading text file. | 
|[NewTxtLoadOptions_AbstractTextLoadOptions](./newtxtloadoptions_abstracttextloadoptions/) | Constructs from a parent object. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetSeparator](./getseparator/) | Gets and sets character separator of text file. | 
|[SetSeparator](./setseparator/) | Gets and sets character separator of text file. | 
|[GetSeparatorString](./getseparatorstring/) | Gets and sets a string value as separator. | 
|[SetSeparatorString](./setseparatorstring/) | Gets and sets a string value as separator. | 
|[IsMultiEncoded](./ismultiencoded/) | True means that the file contains several encoding. | 
|[SetIsMultiEncoded](./setismultiencoded/) | True means that the file contains several encoding. | 
|[GetHasFormula](./gethasformula/) | Indicates whether the text is formula if it starts with "=". | 
|[SetHasFormula](./sethasformula/) | Indicates whether the text is formula if it starts with "=". | 
|[GetHasTextQualifier](./gethastextqualifier/) | Whether there is text qualifier for cell value. Default is true. | 
|[SetHasTextQualifier](./sethastextqualifier/) | Whether there is text qualifier for cell value. Default is true. | 
|[GetTextQualifier](./gettextqualifier/) | Specifies the text qualifier for cell values. Default qualifier is '"'. | 
|[SetTextQualifier](./settextqualifier/) | Specifies the text qualifier for cell values. Default qualifier is '"'. | 
|[GetTreatConsecutiveDelimitersAsOne](./gettreatconsecutivedelimitersasone/) | Whether consecutive delimiters should be treated as one. | 
|[SetTreatConsecutiveDelimitersAsOne](./settreatconsecutivedelimitersasone/) | Whether consecutive delimiters should be treated as one. | 
|[GetTreatQuotePrefixAsValue](./gettreatquoteprefixasvalue/) | Indicates whether the leading single quote sign should be taken as part of the value of one cell.Default is true. If it is false, the leading single quote will be removed from corresponding cell's valueand Style.QuotePrefix will be set as true for the cell. | 
|[SetTreatQuotePrefixAsValue](./settreatquoteprefixasvalue/) | Indicates whether the leading single quote sign should be taken as part of the value of one cell.Default is true. If it is false, the leading single quote will be removed from corresponding cell's valueand Style.QuotePrefix will be set as true for the cell. | 
|[GetExtendToNextSheet](./getextendtonextsheet/) | Whether extends data to next sheet when the rows or columns of data exceed limit.Default is false. | 
|[SetExtendToNextSheet](./setextendtonextsheet/) | Whether extends data to next sheet when the rows or columns of data exceed limit.Default is false. | 
|[GetHeaderRowsCount](./getheaderrowscount/) | The count of header rows to be repeated for extended sheets. | 
|[SetHeaderRowsCount](./setheaderrowscount/) | The count of header rows to be repeated for extended sheets. | 
|[GetHeaderColumnsCount](./getheadercolumnscount/) | The count of header columns to be repeated for extended sheets. | 
|[SetHeaderColumnsCount](./setheadercolumnscount/) | The count of header columns to be repeated for extended sheets. | 
|[GetMaxRowCount](./getmaxrowcount/) | The maximum count of rows to be imported for one sheet. | 
|[SetMaxRowCount](./setmaxrowcount/) | The maximum count of rows to be imported for one sheet. | 
|[GetMaxColumnCount](./getmaxcolumncount/) | The maximum count of columns to be imported for one sheet. | 
|[SetMaxColumnCount](./setmaxcolumncount/) | The maximum count of columns to be imported for one sheet. | 
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
