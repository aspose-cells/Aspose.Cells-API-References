---
title: "DbfLoadOptions Class"
linktitle: "DbfLoadOptions"
articleTitle: "DbfLoadOptions"
second_title: "Aspose.Cells for Python via Java"
description: ""
type: docs
weight: 1670
url: /python-java/asposecells.api/dbfloadoptions/
---

## DbfLoadOptions class

## Constructors

| Name | Description |
| --- | --- |
| [DbfLoadOptions](#constructor) |  |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [LoadFormat](#loadformat) | int | Gets the load format. The value of the property is LoadFormat integer constant. |
| [Password](#password) | String | Gets and set the password of the workbook. |
| [ParsingFormulaOnOpen](#parsingformulaonopen) | boolean | Indicates whether parsing the formula when reading the file. Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file becau |
| [ParsingPivotCachedRecords](#parsingpivotcachedrecords) | boolean | Indicates whether parsing pivot cached records when loading the file. The default value is false. Only applies for Excel |
| [LanguageCode](#languagecode) | int | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. The value |
| [Region](#region) | int | Gets or sets the system regional settings based on CountryCode at the time the file was loaded. The value of the propert |
| [Locale](#locale) | Locale | Gets and sets the Locale used for workbook at the time the file was loaded. |
| [DefaultStyleSettings](#defaultstylesettings) | DefaultStyleSettings | Gets the default style settings for initializing styles of the workbook |
| [StandardFont](#standardfont) | String | Sets the default standard font name NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This pr |
| [StandardFontSize](#standardfontsize) | float | Sets the default standard font size. NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This p |
| [InterruptMonitor](#interruptmonitor) | AbstractInterruptMonitor | Gets and sets the interrupt monitor. |
| [IgnoreNotPrinted](#ignorenotprinted) | boolean | Ignore the data which are not printed if directly printing the file Only for xlsx file. |
| [CheckDataValid](#checkdatavalid) | boolean | Check whether data is valid in the template file. |
| [CheckExcelRestriction](#checkexcelrestriction) | boolean | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputt |
| [KeepUnparsedData](#keepunparseddata) | boolean | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. For sce |
| [LoadFilter](#loadfilter) | LoadFilter | The filter to denote how to load data. |
| [LightCellsDataHandler](#lightcellsdatahandler) | LightCellsDataHandler | The data handler for processing cells data when reading template file. |
| [MemorySetting](#memorysetting) | int | Gets or sets the memory usage options. The value of the property is MemorySetting integer constant. |
| [WarningCallback](#warningcallback) | IWarningCallback | Gets or sets warning callback. |
| [AutoFitterOptions](#autofitteroptions) | AutoFitterOptions | Gets and sets the auto fitter options Only for xlsx ,spreadsheetML file now. |
| [AutoFilter](#autofilter) | boolean | Indicates whether auto filtering the data when loading the files. Sometimes although autofilter is set, the correspondin |
| [FontConfigs](#fontconfigs) | IndividualFontConfigs | Gets and sets individual font configs. Only works for the Workbook which uses this LoadOptions to load. |
| [IgnoreUselessShapes](#ignoreuselessshapes) | boolean | Indicates whether ignoring useless shapes. Only works for xlsx,xlsb, and xlsm files. There are many overlapping identica |
| [PreservePaddingSpacesInFormula](#preservepaddingspacesinformula) | boolean | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting |

## Methods

| Name | Description |
| --- | --- |
| [setPaperSize](#setpapersize) | Sets the default print paper size from default printer's setting.

If there is no setting about paper size,MS Excel will |

### DbfLoadOptions() {#constructor}

### DbfLoadOptions.LoadFormat property {#loadformat}

Gets the load format. The value of the property is LoadFormat integer constant.

**Type:** int

### DbfLoadOptions.Password property {#password}

Gets and set the password of the workbook.

**Type:** String

### DbfLoadOptions.ParsingFormulaOnOpen property {#parsingformulaonopen}

Indicates whether parsing the formula when reading the file. Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file because the formulas in the files are stored with a string formula.

**Type:** boolean

### DbfLoadOptions.ParsingPivotCachedRecords property {#parsingpivotcachedrecords}

Indicates whether parsing pivot cached records when loading the file. The default value is false. Only applies for Excel Xlsx, Xltx, Xltm , Xlsm and xlsb file

**Type:** boolean

### DbfLoadOptions.LanguageCode property {#languagecode}

Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. The value of the property is CountryCode integer constant.

**Type:** int

### DbfLoadOptions.Region property {#region}

Gets or sets the system regional settings based on CountryCode at the time the file was loaded. The value of the property is CountryCode integer constant. If you do not want to use the region saved in the file, please reset it after reading the file.

**Type:** int

### DbfLoadOptions.Locale property {#locale}

Gets and sets the Locale used for workbook at the time the file was loaded.

**Type:** Locale

### DbfLoadOptions.DefaultStyleSettings property {#defaultstylesettings}

Gets the default style settings for initializing styles of the workbook

**Type:** DefaultStyleSettings

### DbfLoadOptions.StandardFont property {#standardfont}

Sets the default standard font name NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.

**Type:** String

### DbfLoadOptions.StandardFontSize property {#standardfontsize}

Sets the default standard font size. NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.

**Type:** float

### DbfLoadOptions.InterruptMonitor property {#interruptmonitor}

Gets and sets the interrupt monitor.

**Type:** AbstractInterruptMonitor

### DbfLoadOptions.IgnoreNotPrinted property {#ignorenotprinted}

Ignore the data which are not printed if directly printing the file Only for xlsx file.

**Type:** boolean

### DbfLoadOptions.CheckDataValid property {#checkdatavalid}

Check whether data is valid in the template file.

**Type:** boolean

### DbfLoadOptions.CheckExcelRestriction property {#checkexcelrestriction}

Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.

**Type:** boolean

### DbfLoadOptions.KeepUnparsedData property {#keepunparseddata}

Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. For scenarios that user only needs to read some contents from template file and does not need to save the workbook back, set this property as false may improve performance, especially when using it together with some kind of LoadFilter,

**Type:** boolean

### DbfLoadOptions.LoadFilter property {#loadfilter}

The filter to denote how to load data.

**Type:** LoadFilter

### DbfLoadOptions.LightCellsDataHandler property {#lightcellsdatahandler}

The data handler for processing cells data when reading template file.

**Type:** LightCellsDataHandler

### DbfLoadOptions.MemorySetting property {#memorysetting}

Gets or sets the memory usage options. The value of the property is MemorySetting integer constant.

**Type:** int

### DbfLoadOptions.WarningCallback property {#warningcallback}

Gets or sets warning callback.

**Type:** IWarningCallback

### DbfLoadOptions.AutoFitterOptions property {#autofitteroptions}

Gets and sets the auto fitter options Only for xlsx ,spreadsheetML file now.

**Type:** AutoFitterOptions

### DbfLoadOptions.AutoFilter property {#autofilter}

Indicates whether auto filtering the data when loading the files. Sometimes although autofilter is set, the corresponding rows is not hidden in the file. Now only works for SpreadSheetML file.

**Type:** boolean

### DbfLoadOptions.FontConfigs property {#fontconfigs}

Gets and sets individual font configs. Only works for the Workbook which uses this LoadOptions to load.

**Type:** IndividualFontConfigs

### DbfLoadOptions.IgnoreUselessShapes property {#ignoreuselessshapes}

Indicates whether ignoring useless shapes. Only works for xlsx,xlsb, and xlsm files. There are many overlapping identical shapes which are useless in some files, we can ingore them when loading files.

**Type:** boolean

### DbfLoadOptions.PreservePaddingSpacesInFormula property {#preservepaddingspacesinformula}

Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. After loading workbook from template file with this option, FormulaSettings.PreservePaddingSpaces will be set to the same value with this property.

**Type:** boolean

### setPaperSize(type) {#setpapersize}

Sets the default print paper size from default printer's setting.

If there is no setting about paper size,MS Excel will use default printer's setting.

| Parameter | Type | Description |
| --- | --- | --- |
| type | int | A PaperSizeType value. The default paper size. |
