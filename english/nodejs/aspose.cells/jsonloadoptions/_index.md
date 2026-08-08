---
title: "JsonLoadOptions"
linktitle: "JsonLoadOptions"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents the options of loading json files"
type: docs
weight: 1950
url: /nodejs/aspose.cells/jsonloadoptions/
---

## JsonLoadOptions class

Represents the options of loading json files

```js
new JsonLoadOptions()
```

Creates an options of loading the file.

## Methods

| Name | Description |
| --- | --- |
| [getAutoFilter()](./getautofilter/) | Indicates whether auto filtering the data when loading the files. Sometimes although autofilter is set, the correspondin |
| [getAutoFitterOptions()](./getautofitteroptions/) | Gets and sets the auto fitter options Only for xlsx ,spreadsheetML file now. |
| [getCheckDataValid()](./getcheckdatavalid/) | Check whether data is valid in the template file. |
| [getCheckExcelRestriction()](./getcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputt |
| [getDefaultStyleSettings()](./getdefaultstylesettings/) | Gets the default style settings for initializing styles of the workbook |
| [getFontConfigs()](./getfontconfigs/) | Gets and sets individual font configs. Only works for the Workbook which uses this LoadOptions to load. |
| [getIgnoreNotPrinted()](./getignorenotprinted/) | Ignore the data which are not printed if directly printing the file Only for xlsx file. |
| [getIgnoreUselessShapes()](./getignoreuselessshapes/) | Indicates whether ignoring useless shapes. Only works for xlsx,xlsb, and xlsm files. There are many overlapping identica |
| [getInterruptMonitor()](./getinterruptmonitor/) | Gets and sets the interrupt monitor. |
| [getKeepUnparsedData()](./getkeepunparseddata/) | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. For sce |
| [getKeptSchema()](./getkeptschema/) |  |
| [getLanguageCode()](./getlanguagecode/) | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. The value |
| [getLayoutOptions()](./getlayoutoptions/) | The options of import json. |
| [getLightCellsDataHandler()](./getlightcellsdatahandler/) | The data handler for processing cells data when reading template file. |
| [getLoadFilter()](./getloadfilter/) | The filter to denote how to load data. |
| [getLoadFormat()](./getloadformat/) | Gets the load format. The value of the property is LoadFormat integer constant. |
| [getLocale()](./getlocale/) | Gets and sets the Locale used for workbook at the time the file was loaded. |
| [getMemorySetting()](./getmemorysetting/) | Gets or sets the memory usage options. The value of the property is MemorySetting integer constant. |
| [getMultipleWorksheets()](./getmultipleworksheets/) | Indicates whether importing each attribute of JsonObject object as one worksheet when all child nodes are array nodes. |
| [getParsingFormulaOnOpen()](./getparsingformulaonopen/) | Indicates whether parsing the formula when reading the file. Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file becau |
| [getParsingPivotCachedRecords()](./getparsingpivotcachedrecords/) | Indicates whether parsing pivot cached records when loading the file. The default value is false. Only applies for Excel |
| [getPassword()](./getpassword/) | Gets and set the password of the workbook. |
| [getPreservePaddingSpacesInFormula()](./getpreservepaddingspacesinformula/) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting |
| [getRegion()](./getregion/) | Gets or sets the system regional settings based on CountryCode at the time the file was loaded. The value of the propert |
| [getStandardFont()](./getstandardfont/) | Sets the default standard font name NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This pr |
| [getStandardFontSize()](./getstandardfontsize/) | Sets the default standard font size. NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This p |
| [getStartCell()](./getstartcell/) | Gets and sets the start cell. |
| [getWarningCallback()](./getwarningcallback/) | Gets or sets warning callback. |
| [setAutoFilter()](./setautofilter/) | Indicates whether auto filtering the data when loading the files. Sometimes although autofilter is set, the correspondin |
| [setAutoFitterOptions()](./setautofitteroptions/) | Gets and sets the auto fitter options Only for xlsx ,spreadsheetML file now. |
| [setCheckDataValid()](./setcheckdatavalid/) | Check whether data is valid in the template file. |
| [setCheckExcelRestriction()](./setcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputt |
| [setFontConfigs()](./setfontconfigs/) | Gets and sets individual font configs. Only works for the Workbook which uses this LoadOptions to load. |
| [setIgnoreNotPrinted()](./setignorenotprinted/) | Ignore the data which are not printed if directly printing the file Only for xlsx file. |
| [setIgnoreUselessShapes()](./setignoreuselessshapes/) | Indicates whether ignoring useless shapes. Only works for xlsx,xlsb, and xlsm files. There are many overlapping identica |
| [setInterruptMonitor()](./setinterruptmonitor/) | Gets and sets the interrupt monitor. |
| [setKeepUnparsedData()](./setkeepunparseddata/) | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. For sce |
| [setKeptSchema()](./setkeptschema/) |  |
| [setLanguageCode()](./setlanguagecode/) | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. The value |
| [setLayoutOptions()](./setlayoutoptions/) | The options of import json. |
| [setLightCellsDataHandler()](./setlightcellsdatahandler/) | The data handler for processing cells data when reading template file. |
| [setLoadFilter()](./setloadfilter/) | The filter to denote how to load data. |
| [setLocale()](./setlocale/) | Gets and sets the Locale used for workbook at the time the file was loaded. |
| [setMemorySetting()](./setmemorysetting/) | Gets or sets the memory usage options. The value of the property is MemorySetting integer constant. |
| [setMultipleWorksheets()](./setmultipleworksheets/) | Indicates whether importing each attribute of JsonObject object as one worksheet when all child nodes are array nodes. |
| [setPaperSize(type)](./setpapersize/) | Sets the default print paper size from default printer's setting. If there is no setting about paper size,MS Excel will  |
| [setParsingFormulaOnOpen()](./setparsingformulaonopen/) | Indicates whether parsing the formula when reading the file. Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file becau |
| [setParsingPivotCachedRecords()](./setparsingpivotcachedrecords/) | Indicates whether parsing pivot cached records when loading the file. The default value is false. Only applies for Excel |
| [setPassword()](./setpassword/) | Gets and set the password of the workbook. |
| [setPreservePaddingSpacesInFormula()](./setpreservepaddingspacesinformula/) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting |
| [setRegion()](./setregion/) | Gets or sets the system regional settings based on CountryCode at the time the file was loaded. The value of the propert |
| [setStandardFont()](./setstandardfont/) | Sets the default standard font name NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This pr |
| [setStandardFontSize()](./setstandardfontsize/) | Sets the default standard font size. NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This p |
| [setStartCell()](./setstartcell/) | Gets and sets the start cell. |
| [setWarningCallback()](./setwarningcallback/) | Gets or sets warning callback. |
