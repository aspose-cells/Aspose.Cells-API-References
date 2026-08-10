---
title: "XmlLoadOptions Class"
linktitle: "XmlLoadOptions"
articleTitle: "XmlLoadOptions"
second_title: "Aspose.Cells for Python via Java"
description: "Represents the options of loading xml."
type: docs
weight: 7670
url: /python-java/asposecells.api/xmlloadoptions/
---

## XmlLoadOptions class

Represents the options of loading xml.

## Constructors

| Name | Description |
| --- | --- |
| [XmlLoadOptions](#constructor) | Represents the options of loading xml file. |
| [XmlLoadOptions](#constructor) | Represents the options of loading xml file. |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [StartCell](#startcell) | String | Gets and sets the start cell. Only works when the file is not speadsheetML or mapping xml to Excel. |
| [IsXmlMap](#isxmlmap) | boolean | Indicates whether mapping xml to Excel. The default value is false. |
| [ContainsMultipleWorksheets](#containsmultipleworksheets) | boolean | Indicates whether importing xml as multiple worksheets. |
| [ConvertNumericOrDate](#convertnumericordate) | boolean | Indicates whether converting the value in xml file to numeric or date. |
| [NumberFormat](#numberformat) | String | Gets and sets the format of numeric value. |
| [DateFormat](#dateformat) | String | Gets and sets the format of date value. |
| [IgnoreRootAttributes](#ignorerootattributes) | boolean | Indicates whether ignore attributes of the root element. |
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

### XmlLoadOptions() (1 of 2) {#constructor}

Represents the options of loading xml file.

---

### XmlLoadOptions(type) (2 of 2) {#constructor-1}

Represents the options of loading xml file.

| Parameter | Type | Description |
| --- | --- | --- |
| type | int | A LoadFormat value. The load format type. |

### XmlLoadOptions.StartCell property {#startcell}

Gets and sets the start cell. Only works when the file is not speadsheetML or mapping xml to Excel.

**Type:** String

### XmlLoadOptions.IsXmlMap property {#isxmlmap}

Indicates whether mapping xml to Excel. The default value is false.

**Type:** boolean

### XmlLoadOptions.ContainsMultipleWorksheets property {#containsmultipleworksheets}

Indicates whether importing xml as multiple worksheets.

**Type:** boolean

### XmlLoadOptions.ConvertNumericOrDate property {#convertnumericordate}

Indicates whether converting the value in xml file to numeric or date.

**Type:** boolean

### XmlLoadOptions.NumberFormat property {#numberformat}

Gets and sets the format of numeric value.

**Type:** String

### XmlLoadOptions.DateFormat property {#dateformat}

Gets and sets the format of date value.

**Type:** String

### XmlLoadOptions.IgnoreRootAttributes property {#ignorerootattributes}

Indicates whether ignore attributes of the root element.

**Type:** boolean

### XmlLoadOptions.LoadFormat property {#loadformat}

Gets the load format. The value of the property is LoadFormat integer constant.

**Type:** int

### XmlLoadOptions.Password property {#password}

Gets and set the password of the workbook.

**Type:** String

### XmlLoadOptions.ParsingFormulaOnOpen property {#parsingformulaonopen}

Indicates whether parsing the formula when reading the file. Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file because the formulas in the files are stored with a string formula.

**Type:** boolean

### XmlLoadOptions.ParsingPivotCachedRecords property {#parsingpivotcachedrecords}

Indicates whether parsing pivot cached records when loading the file. The default value is false. Only applies for Excel Xlsx, Xltx, Xltm , Xlsm and xlsb file

**Type:** boolean

### XmlLoadOptions.LanguageCode property {#languagecode}

Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. The value of the property is CountryCode integer constant.

**Type:** int

### XmlLoadOptions.Region property {#region}

Gets or sets the system regional settings based on CountryCode at the time the file was loaded. The value of the property is CountryCode integer constant. If you do not want to use the region saved in the file, please reset it after reading the file.

**Type:** int

### XmlLoadOptions.Locale property {#locale}

Gets and sets the Locale used for workbook at the time the file was loaded.

**Type:** Locale

### XmlLoadOptions.DefaultStyleSettings property {#defaultstylesettings}

Gets the default style settings for initializing styles of the workbook

**Type:** DefaultStyleSettings

### XmlLoadOptions.StandardFont property {#standardfont}

Sets the default standard font name NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.

**Type:** String

### XmlLoadOptions.StandardFontSize property {#standardfontsize}

Sets the default standard font size. NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.

**Type:** float

### XmlLoadOptions.InterruptMonitor property {#interruptmonitor}

Gets and sets the interrupt monitor.

**Type:** AbstractInterruptMonitor

### XmlLoadOptions.IgnoreNotPrinted property {#ignorenotprinted}

Ignore the data which are not printed if directly printing the file Only for xlsx file.

**Type:** boolean

### XmlLoadOptions.CheckDataValid property {#checkdatavalid}

Check whether data is valid in the template file.

**Type:** boolean

### XmlLoadOptions.CheckExcelRestriction property {#checkexcelrestriction}

Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.

**Type:** boolean

### XmlLoadOptions.KeepUnparsedData property {#keepunparseddata}

Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. For scenarios that user only needs to read some contents from template file and does not need to save the workbook back, set this property as false may improve performance, especially when using it together with some kind of LoadFilter,

**Type:** boolean

### XmlLoadOptions.LoadFilter property {#loadfilter}

The filter to denote how to load data.

**Type:** LoadFilter

### XmlLoadOptions.LightCellsDataHandler property {#lightcellsdatahandler}

The data handler for processing cells data when reading template file.

**Type:** LightCellsDataHandler

### XmlLoadOptions.MemorySetting property {#memorysetting}

Gets or sets the memory usage options. The value of the property is MemorySetting integer constant.

**Type:** int

### XmlLoadOptions.WarningCallback property {#warningcallback}

Gets or sets warning callback.

**Type:** IWarningCallback

### XmlLoadOptions.AutoFitterOptions property {#autofitteroptions}

Gets and sets the auto fitter options Only for xlsx ,spreadsheetML file now.

**Type:** AutoFitterOptions

### XmlLoadOptions.AutoFilter property {#autofilter}

Indicates whether auto filtering the data when loading the files. Sometimes although autofilter is set, the corresponding rows is not hidden in the file. Now only works for SpreadSheetML file.

**Type:** boolean

### XmlLoadOptions.FontConfigs property {#fontconfigs}

Gets and sets individual font configs. Only works for the Workbook which uses this LoadOptions to load.

**Type:** IndividualFontConfigs

### XmlLoadOptions.IgnoreUselessShapes property {#ignoreuselessshapes}

Indicates whether ignoring useless shapes. Only works for xlsx,xlsb, and xlsm files. There are many overlapping identical shapes which are useless in some files, we can ingore them when loading files.

**Type:** boolean

### XmlLoadOptions.PreservePaddingSpacesInFormula property {#preservepaddingspacesinformula}

Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. After loading workbook from template file with this option, FormulaSettings.PreservePaddingSpaces will be set to the same value with this property.

**Type:** boolean

### setPaperSize(type) {#setpapersize}

Sets the default print paper size from default printer's setting.

If there is no setting about paper size,MS Excel will use default printer's setting.

| Parameter | Type | Description |
| --- | --- | --- |
| type | int | A PaperSizeType value. The default paper size. |
