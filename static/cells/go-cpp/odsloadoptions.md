##OdsLoadOptions Class
'OdsLoadOptions class. Encapsulates the object that represents odsloadoptions in Go.'
## OdsLoadOptions class
Represents the options of loading ods file.
```go
type OdsLoadOptions struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewOdsLoadOptions](./newodsloadoptions/) | Represents the options of loading ods file. |
|[NewOdsLoadOptions_LoadFormat](./newodsloadoptions_loadformat/) | Represents the options of loading ods file. |
|[NewOdsLoadOptions_LoadOptions](./newodsloadoptions_loadoptions/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetApplyExcelDefaultStyleToHyperlink](./getapplyexceldefaultstyletohyperlink/) | Indicates whether applying the default style of the Excel to hyperlink. |
|[SetApplyExcelDefaultStyleToHyperlink](./setapplyexceldefaultstyletohyperlink/) | Indicates whether applying the default style of the Excel to hyperlink. |
|[GetRefreshPivotTables](./getrefreshpivottables/) | Indicates whether refresh pivot tables when loading file. |
|[SetRefreshPivotTables](./setrefreshpivottables/) | Indicates whether refresh pivot tables when loading file. |
|[IsClassicPivotTable](./isclassicpivottable/) | Indicates whether the pivot table is classic. |
|[SetIsClassicPivotTable](./setisclassicpivottable/) | Indicates whether the pivot table is classic. |
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
