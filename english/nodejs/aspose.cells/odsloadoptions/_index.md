---
title: "OdsLoadOptions"
linktitle: "OdsLoadOptions"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents the options of loading ods file."
type: docs
weight: 2400
url: /nodejs/aspose.cells/odsloadoptions/
---

## OdsLoadOptions class

Represents the options of loading ods file.

```js
new OdsLoadOptions()
```

Represents the options of loading ods file.

## Methods

| Name | Description |
| --- | --- |
| [constructor_overload$1(type)](#constructor-overload1) | Represents the options of loading ods file. |
| [getApplyExcelDefaultStyleToHyperlink()](#getapplyexceldefaultstyletohyperlink) | Indicates whether applying the default style of the Excel to hyperlink. |
| [getAutoFilter()](#getautofilter) | Indicates whether auto filtering the data when loading the files. Sometimes although autofilter is set, the correspondin |
| [getAutoFitterOptions()](#getautofitteroptions) | Gets and sets the auto fitter options Only for xlsx ,spreadsheetML file now. |
| [getCheckDataValid()](#getcheckdatavalid) | Check whether data is valid in the template file. |
| [getCheckExcelRestriction()](#getcheckexcelrestriction) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputt |
| [getDefaultStyleSettings()](#getdefaultstylesettings) | Gets the default style settings for initializing styles of the workbook |
| [getFontConfigs()](#getfontconfigs) | Gets and sets individual font configs. Only works for the Workbook which uses this LoadOptions to load. |
| [getIgnoreNotPrinted()](#getignorenotprinted) | Ignore the data which are not printed if directly printing the file Only for xlsx file. |
| [getIgnoreUselessShapes()](#getignoreuselessshapes) | Indicates whether ignoring useless shapes. Only works for xlsx,xlsb, and xlsm files. There are many overlapping identica |
| [getInterruptMonitor()](#getinterruptmonitor) | Gets and sets the interrupt monitor. |
| [getKeepUnparsedData()](#getkeepunparseddata) | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. For sce |
| [getLanguageCode()](#getlanguagecode) | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. The value |
| [getLightCellsDataHandler()](#getlightcellsdatahandler) | The data handler for processing cells data when reading template file. |
| [getLoadFilter()](#getloadfilter) | The filter to denote how to load data. |
| [getLoadFormat()](#getloadformat) | Gets the load format. The value of the property is LoadFormat integer constant. |
| [getLocale()](#getlocale) | Gets and sets the Locale used for workbook at the time the file was loaded. |
| [getMemorySetting()](#getmemorysetting) | Gets or sets the memory usage options. The value of the property is MemorySetting integer constant. |
| [getParsingFormulaOnOpen()](#getparsingformulaonopen) | Indicates whether parsing the formula when reading the file. Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file becau |
| [getParsingPivotCachedRecords()](#getparsingpivotcachedrecords) | Indicates whether parsing pivot cached records when loading the file. The default value is false. Only applies for Excel |
| [getPassword()](#getpassword) | Gets and set the password of the workbook. |
| [getPreservePaddingSpacesInFormula()](#getpreservepaddingspacesinformula) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting |
| [getRefreshPivotTables()](#getrefreshpivottables) | Indicates whether refresh pivot tables when loading file. |
| [getRegion()](#getregion) | Gets or sets the system regional settings based on CountryCode at the time the file was loaded. The value of the propert |
| [getStandardFont()](#getstandardfont) | Sets the default standard font name NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This pr |
| [getStandardFontSize()](#getstandardfontsize) | Sets the default standard font size. NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This p |
| [getWarningCallback()](#getwarningcallback) | Gets or sets warning callback. |
| [isClassicPivotTable()](#isclassicpivottable) |  |
| [setApplyExcelDefaultStyleToHyperlink()](#setapplyexceldefaultstyletohyperlink) | Indicates whether applying the default style of the Excel to hyperlink. |
| [setAutoFilter()](#setautofilter) | Indicates whether auto filtering the data when loading the files. Sometimes although autofilter is set, the correspondin |
| [setAutoFitterOptions()](#setautofitteroptions) | Gets and sets the auto fitter options Only for xlsx ,spreadsheetML file now. |
| [setCheckDataValid()](#setcheckdatavalid) | Check whether data is valid in the template file. |
| [setCheckExcelRestriction()](#setcheckexcelrestriction) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputt |
| [setClassicPivotTable()](#setclassicpivottable) |  |
| [setFontConfigs()](#setfontconfigs) | Gets and sets individual font configs. Only works for the Workbook which uses this LoadOptions to load. |
| [setIgnoreNotPrinted()](#setignorenotprinted) | Ignore the data which are not printed if directly printing the file Only for xlsx file. |
| [setIgnoreUselessShapes()](#setignoreuselessshapes) | Indicates whether ignoring useless shapes. Only works for xlsx,xlsb, and xlsm files. There are many overlapping identica |
| [setInterruptMonitor()](#setinterruptmonitor) | Gets and sets the interrupt monitor. |
| [setKeepUnparsedData()](#setkeepunparseddata) | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. For sce |
| [setLanguageCode()](#setlanguagecode) | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. The value |
| [setLightCellsDataHandler()](#setlightcellsdatahandler) | The data handler for processing cells data when reading template file. |
| [setLoadFilter()](#setloadfilter) | The filter to denote how to load data. |
| [setLocale()](#setlocale) | Gets and sets the Locale used for workbook at the time the file was loaded. |
| [setMemorySetting()](#setmemorysetting) | Gets or sets the memory usage options. The value of the property is MemorySetting integer constant. |
| [setPaperSize(type)](#setpapersize) | Sets the default print paper size from default printer's setting. If there is no setting about paper size,MS Excel will  |
| [setParsingFormulaOnOpen()](#setparsingformulaonopen) | Indicates whether parsing the formula when reading the file. Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file becau |
| [setParsingPivotCachedRecords()](#setparsingpivotcachedrecords) | Indicates whether parsing pivot cached records when loading the file. The default value is false. Only applies for Excel |
| [setPassword()](#setpassword) | Gets and set the password of the workbook. |
| [setPreservePaddingSpacesInFormula()](#setpreservepaddingspacesinformula) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting |
| [setRefreshPivotTables()](#setrefreshpivottables) | Indicates whether refresh pivot tables when loading file. |
| [setRegion()](#setregion) | Gets or sets the system regional settings based on CountryCode at the time the file was loaded. The value of the propert |
| [setStandardFont()](#setstandardfont) | Sets the default standard font name NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This pr |
| [setStandardFontSize()](#setstandardfontsize) | Sets the default standard font size. NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This p |
| [setWarningCallback()](#setwarningcallback) | Gets or sets warning callback. |

### constructor_overload$1(type) {#constructor-overload1}

Represents the options of loading ods file.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | LoadFormat |

### getApplyExcelDefaultStyleToHyperlink() {#getapplyexceldefaultstyletohyperlink}

Indicates whether applying the default style of the Excel to hyperlink.

### getAutoFilter() {#getautofilter}

Indicates whether auto filtering the data when loading the files. Sometimes although autofilter is set, the corresponding rows is not hidden in the file. Now only works for SpreadSheetML file.

### getAutoFitterOptions() {#getautofitteroptions}

Gets and sets the auto fitter options Only for xlsx ,spreadsheetML file now.

### getCheckDataValid() {#getcheckdatavalid}

Check whether data is valid in the template file.

### getCheckExcelRestriction() {#getcheckexcelrestriction}

Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.

### getDefaultStyleSettings() {#getdefaultstylesettings}

Gets the default style settings for initializing styles of the workbook

### getFontConfigs() {#getfontconfigs}

Gets and sets individual font configs. Only works for the Workbook which uses this LoadOptions to load.

### getIgnoreNotPrinted() {#getignorenotprinted}

Ignore the data which are not printed if directly printing the file Only for xlsx file.

### getIgnoreUselessShapes() {#getignoreuselessshapes}

Indicates whether ignoring useless shapes. Only works for xlsx,xlsb, and xlsm files. There are many overlapping identical shapes which are useless in some files, we can ingore them when loading files.

### getInterruptMonitor() {#getinterruptmonitor}

Gets and sets the interrupt monitor.

### getKeepUnparsedData() {#getkeepunparseddata}

Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. For scenarios that user only needs to read some contents from template file and does not need to save the workbook back, set this property as false may improve performance, especially when using it together with some kind of LoadFilter,

### getLanguageCode() {#getlanguagecode}

Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. The value of the property is CountryCode integer constant.

### getLightCellsDataHandler() {#getlightcellsdatahandler}

The data handler for processing cells data when reading template file.

### getLoadFilter() {#getloadfilter}

The filter to denote how to load data.

### getLoadFormat() {#getloadformat}

Gets the load format. The value of the property is LoadFormat integer constant.

### getLocale() {#getlocale}

Gets and sets the Locale used for workbook at the time the file was loaded.

### getMemorySetting() {#getmemorysetting}

Gets or sets the memory usage options. The value of the property is MemorySetting integer constant.

### getParsingFormulaOnOpen() {#getparsingformulaonopen}

Indicates whether parsing the formula when reading the file. Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file because the formulas in the files are stored with a string formula.

### getParsingPivotCachedRecords() {#getparsingpivotcachedrecords}

Indicates whether parsing pivot cached records when loading the file. The default value is false. Only applies for Excel Xlsx, Xltx, Xltm , Xlsm and xlsb file

### getPassword() {#getpassword}

Gets and set the password of the workbook.

### getPreservePaddingSpacesInFormula() {#getpreservepaddingspacesinformula}

Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. After loading workbook from template file with this option, FormulaSettings.PreservePaddingSpaces will be set to the same value with this property.

### getRefreshPivotTables() {#getrefreshpivottables}

Indicates whether refresh pivot tables when loading file.

### getRegion() {#getregion}

Gets or sets the system regional settings based on CountryCode at the time the file was loaded. The value of the property is CountryCode integer constant.If you do not want to use the region saved in the file, please reset it after reading the file.

### getStandardFont() {#getstandardfont}

Sets the default standard font name NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.

### getStandardFontSize() {#getstandardfontsize}

Sets the default standard font size. NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.

### getWarningCallback() {#getwarningcallback}

Gets or sets warning callback.

### isClassicPivotTable() {#isclassicpivottable}

### setApplyExcelDefaultStyleToHyperlink() {#setapplyexceldefaultstyletohyperlink}

Indicates whether applying the default style of the Excel to hyperlink.

### setAutoFilter() {#setautofilter}

Indicates whether auto filtering the data when loading the files. Sometimes although autofilter is set, the corresponding rows is not hidden in the file. Now only works for SpreadSheetML file.

### setAutoFitterOptions() {#setautofitteroptions}

Gets and sets the auto fitter options Only for xlsx ,spreadsheetML file now.

### setCheckDataValid() {#setcheckdatavalid}

Check whether data is valid in the template file.

### setCheckExcelRestriction() {#setcheckexcelrestriction}

Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.

### setClassicPivotTable() {#setclassicpivottable}

### setFontConfigs() {#setfontconfigs}

Gets and sets individual font configs. Only works for the Workbook which uses this LoadOptions to load.

### setIgnoreNotPrinted() {#setignorenotprinted}

Ignore the data which are not printed if directly printing the file Only for xlsx file.

### setIgnoreUselessShapes() {#setignoreuselessshapes}

Indicates whether ignoring useless shapes. Only works for xlsx,xlsb, and xlsm files. There are many overlapping identical shapes which are useless in some files, we can ingore them when loading files.

### setInterruptMonitor() {#setinterruptmonitor}

Gets and sets the interrupt monitor.

### setKeepUnparsedData() {#setkeepunparseddata}

Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. For scenarios that user only needs to read some contents from template file and does not need to save the workbook back, set this property as false may improve performance, especially when using it together with some kind of LoadFilter,

### setLanguageCode() {#setlanguagecode}

Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. The value of the property is CountryCode integer constant.

### setLightCellsDataHandler() {#setlightcellsdatahandler}

The data handler for processing cells data when reading template file.

### setLoadFilter() {#setloadfilter}

The filter to denote how to load data.

### setLocale() {#setlocale}

Gets and sets the Locale used for workbook at the time the file was loaded.

### setMemorySetting() {#setmemorysetting}

Gets or sets the memory usage options. The value of the property is MemorySetting integer constant.

### setPaperSize(type) {#setpapersize}

Sets the default print paper size from default printer's setting. If there is no setting about paper size,MS Excel will use default printer's setting.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | PaperSizeType |

### setParsingFormulaOnOpen() {#setparsingformulaonopen}

Indicates whether parsing the formula when reading the file. Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file because the formulas in the files are stored with a string formula.

### setParsingPivotCachedRecords() {#setparsingpivotcachedrecords}

Indicates whether parsing pivot cached records when loading the file. The default value is false. Only applies for Excel Xlsx, Xltx, Xltm , Xlsm and xlsb file

### setPassword() {#setpassword}

Gets and set the password of the workbook.

### setPreservePaddingSpacesInFormula() {#setpreservepaddingspacesinformula}

Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. After loading workbook from template file with this option, FormulaSettings.PreservePaddingSpaces will be set to the same value with this property.

### setRefreshPivotTables() {#setrefreshpivottables}

Indicates whether refresh pivot tables when loading file.

### setRegion() {#setregion}

Gets or sets the system regional settings based on CountryCode at the time the file was loaded. The value of the property is CountryCode integer constant.If you do not want to use the region saved in the file, please reset it after reading the file.

### setStandardFont() {#setstandardfont}

Sets the default standard font name NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.

### setStandardFontSize() {#setstandardfontsize}

Sets the default standard font size. NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.

### setWarningCallback() {#setwarningcallback}

Gets or sets warning callback.
