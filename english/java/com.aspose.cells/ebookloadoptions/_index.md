---
title: EbookLoadOptions
second_title: Aspose.Cells for Java API Reference
description: Represents options when importing an ebook file.
type: docs
url: /java/com.aspose.cells/ebookloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LoadOptions](../../com.aspose.cells/loadoptions), [com.aspose.cells.AbstractTextLoadOptions](../../com.aspose.cells/abstracttextloadoptions), [com.aspose.cells.HtmlLoadOptions](../../com.aspose.cells/htmlloadoptions)
```
public class EbookLoadOptions extends HtmlLoadOptions
```

Represents options when importing an ebook file.
## Constructors

| Constructor | Description |
| --- | --- |
| [EbookLoadOptions()](#EbookLoadOptions--) | Creates an options of loading the ebook file. |
| [EbookLoadOptions(int loadFormat)](#EbookLoadOptions-int-) | Creates an options of loading the ebook file. |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--) | The directory that the attached files will be saved to. |
| [getAutoFilter()](#getAutoFilter--) | Indicates whether auto filtering the data when loading the files. |
| [getAutoFitColsAndRows()](#getAutoFitColsAndRows--) | Indicates whether auto-fit columns and rows. |
| [getAutoFitterOptions()](#getAutoFitterOptions--) | Gets the auto fitter options |
| [getCheckDataValid()](#getCheckDataValid--) | Check whether data is valid in the template file. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Whether check restriction of excel file when user modify cells related objects. |
| [getClass()](#getClass--) |  |
| [getConvertDateTimeData()](#getConvertDateTimeData--) | Gets a value that indicates whether the string in text file is converted to date data. |
| [getConvertFormulasData()](#getConvertFormulasData--) | if true, convert string to formula when string value starts with character '=',the default value is false. |
| [getConvertNumericData()](#getConvertNumericData--) | Gets a value that indicates whether the string in text file is converted to numeric data. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Gets the default style settings for initializing styles of the workbook |
| [getDeleteRedundantSpaces()](#getDeleteRedundantSpaces--) | Indicates whether delete redundant spaces when the text wraps lines using `<br>` tag. |
| [getEncoding()](#getEncoding--) | Gets the default encoding. |
| [getFontConfigs()](#getFontConfigs--) | Gets individual font configs. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Ignore the data which are not printed if directly printing the file |
| [getIgnoreUselessShapes()](#getIgnoreUselessShapes--) | Indicates whether ignoring useless shapes. |
| [getInterruptMonitor()](#getInterruptMonitor--) | Gets the interrupt monitor. |
| [getKeepPrecision()](#getKeepPrecision--) | Indicates whether not parsing a string value if the length is 15. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. |
| [getLanguageCode()](#getLanguageCode--) | Gets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [getLightCellsDataHandler()](#getLightCellsDataHandler--) | The data handler for processing cells data when reading template file. |
| [getLoadFilter()](#getLoadFilter--) | The filter to denote how to load data. |
| [getLoadFormat()](#getLoadFormat--) | Gets the load format. |
| [getLoadFormulas()](#getLoadFormulas--) | Indicates whether importing formulas if the original html file contains formulas |
| [getLoadStyleStrategy()](#getLoadStyleStrategy--) | Indicates the strategy to apply style for parsed values when converting string value to number or datetime. |
| [getLocale()](#getLocale--) | Gets the regional settings used for the Workbook that will be loaded. |
| [getMemorySetting()](#getMemorySetting--) | Gets the memory mode for loaded workbook. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Indicates whether parsing the formula when reading the file. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Indicates whether parsing pivot cached records when loading the file. |
| [getPassword()](#getPassword--) | Gets the password of the workbook. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. |
| [getProgId()](#getProgId--) | Gets the program id of creating the file. |
| [getRegion()](#getRegion--) | Gets the regional settings used for the Workbook that will be loaded. |
| [getStandardFont()](#getStandardFont--) | Sets the default standard font name |
| [getStandardFontSize()](#getStandardFontSize--) | Sets the default standard font size. |
| [getStreamProvider()](#getStreamProvider--) | Gets the StreamProviderImportHtmlFile for importing objects. |
| [getSupportDivTag()](#getSupportDivTag--) | Indicates whether support the layout of `<div>` tag when the html file contains it. |
| [getTableLoadOptions()](#getTableLoadOptions--) | Get the HtmlTableLoadOptionCollection instance |
| [getWarningCallback()](#getWarningCallback--) | Gets warning callback. |
| [hasFormula()](#hasFormula--) | Indicates whether the text is formula if it starts with "=". |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | The directory that the attached files will be saved to. |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Indicates whether auto filtering the data when loading the files. |
| [setAutoFitColsAndRows(boolean value)](#setAutoFitColsAndRows-boolean-) | Indicates whether auto-fit columns and rows. |
| [setAutoFitterOptions(AutoFitterOptions value)](#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-) | Sets the auto fitter options |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Check whether data is valid in the template file. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Whether check restriction of excel file when user modify cells related objects. |
| [setConvertDateTimeData(boolean value)](#setConvertDateTimeData-boolean-) | Sets a value that indicates whether the string in text file is converted to date data. |
| [setConvertFormulasData(boolean value)](#setConvertFormulasData-boolean-) | if true, convert string to formula when string value starts with character '=',the default value is false. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Sets a value that indicates whether the string in text file is converted to numeric data. |
| [setDeleteRedundantSpaces(boolean value)](#setDeleteRedundantSpaces-boolean-) | Indicates whether delete redundant spaces when the text wraps lines using `<br>` tag. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Sets the default encoding. |
| [setFontConfigs(IndividualFontConfigs value)](#setFontConfigs-com.aspose.cells.IndividualFontConfigs-) | Sets individual font configs. |
| [setHasFormula(boolean value)](#setHasFormula-boolean-) | Indicates whether the text is formula if it starts with "=". |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Ignore the data which are not printed if directly printing the file |
| [setIgnoreUselessShapes(boolean value)](#setIgnoreUselessShapes-boolean-) | Indicates whether ignoring useless shapes. |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | Sets the interrupt monitor. |
| [setKeepPrecision(boolean value)](#setKeepPrecision-boolean-) | Indicates whether not parsing a string value if the length is 15. |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Sets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [setLightCellsDataHandler(LightCellsDataHandler value)](#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-) | The data handler for processing cells data when reading template file. |
| [setLoadFilter(LoadFilter value)](#setLoadFilter-com.aspose.cells.LoadFilter-) | The filter to denote how to load data. |
| [setLoadFormulas(boolean value)](#setLoadFormulas-boolean-) | Indicates whether importing formulas if the original html file contains formulas |
| [setLoadStyleStrategy(int value)](#setLoadStyleStrategy-int-) | Indicates the strategy to apply style for parsed values when converting string value to number or datetime. |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | Sets the regional settings used for the Workbook that will be loaded. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Sets the memory mode for loaded workbook. |
| [setPaperSize(int type)](#setPaperSize-int-) | Sets the default print paper size from default printer's setting. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Indicates whether parsing the formula when reading the file. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Indicates whether parsing pivot cached records when loading the file. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Sets the password of the workbook. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. |
| [setRegion(int value)](#setRegion-int-) | Sets the regional settings used for the Workbook that will be loaded. |
| [setStandardFont(String value)](#setStandardFont-java.lang.String-) | Sets the default standard font name |
| [setStandardFontSize(double value)](#setStandardFontSize-double-) | Sets the default standard font size. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | Sets the StreamProviderImportHtmlFile for importing objects. |
| [setSupportDivTag(boolean value)](#setSupportDivTag-boolean-) | Indicates whether support the layout of `<div>` tag when the html file contains it. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Sets warning callback. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### EbookLoadOptions() {#EbookLoadOptions--}
```
public EbookLoadOptions()
```


Creates an options of loading the ebook file.

### EbookLoadOptions(int loadFormat) {#EbookLoadOptions-int-}
```
public EbookLoadOptions(int loadFormat)
```


Creates an options of loading the ebook file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat). The loading format |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAttachedFilesDirectory() {#getAttachedFilesDirectory--}
```
public String getAttachedFilesDirectory()
```


The directory that the attached files will be saved to.

**Remarks**

NOTE: This member is now obsolete. Instead, please use HtmlLoadOptions.StreamProvider property. This property will be removed 12 months later since December 2014. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
java.lang.String
### getAutoFilter() {#getAutoFilter--}
```
public boolean getAutoFilter()
```


Indicates whether auto filtering the data when loading the files.

**Remarks**

Sometimes although autofilter is set, the corresponding rows is not hidden in the file. Now only works for SpreadSheetML file.

**Returns:**
boolean
### getAutoFitColsAndRows() {#getAutoFitColsAndRows--}
```
public boolean getAutoFitColsAndRows()
```


Indicates whether auto-fit columns and rows. The default value is false.

**Returns:**
boolean
### getAutoFitterOptions() {#getAutoFitterOptions--}
```
public AutoFitterOptions getAutoFitterOptions()
```


Gets the auto fitter options

**Remarks**

Only for xlsx ,spreadsheetML file now.

**Returns:**
[AutoFitterOptions](../../com.aspose.cells/autofitteroptions)
### getCheckDataValid() {#getCheckDataValid--}
```
public boolean getCheckDataValid()
```


Check whether data is valid in the template file.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConvertDateTimeData() {#getConvertDateTimeData--}
```
public boolean getConvertDateTimeData()
```


Gets a value that indicates whether the string in text file is converted to date data. Default value is true.

**Returns:**
boolean
### getConvertFormulasData() {#getConvertFormulasData--}
```
public boolean getConvertFormulasData()
```


if true, convert string to formula when string value starts with character '=',the default value is false.

**Remarks**

NOTE: This property is now obsolete. Instead, please use HtmlLoadOptions.HasFormula property. This property will be removed 12 months later since March 2023. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Gets a value that indicates whether the string in text file is converted to numeric data. Default value is true.

**Returns:**
boolean
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```
public DefaultStyleSettings getDefaultStyleSettings()
```


Gets the default style settings for initializing styles of the workbook

**Returns:**
[DefaultStyleSettings](../../com.aspose.cells/defaultstylesettings)
### getDeleteRedundantSpaces() {#getDeleteRedundantSpaces--}
```
public boolean getDeleteRedundantSpaces()
```


Indicates whether delete redundant spaces when the text wraps lines using `<br>` tag. The default value is false.

**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Gets the default encoding. Only applies for csv file.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getFontConfigs() {#getFontConfigs--}
```
public IndividualFontConfigs getFontConfigs()
```


Gets individual font configs. Only works for the [Workbook](../../com.aspose.cells/workbook) which uses this [LoadOptions](../../com.aspose.cells/loadoptions) to load.

**Returns:**
[IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs)
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```


Ignore the data which are not printed if directly printing the file

**Remarks**

Only for xlsx file.

**Returns:**
boolean
### getIgnoreUselessShapes() {#getIgnoreUselessShapes--}
```
public boolean getIgnoreUselessShapes()
```


Indicates whether ignoring useless shapes.

**Remarks**

Only works for xlsx,xlsb, and xlsm files. There are many overlapping identical shapes which are useless in some files, we can ingore them when loading files.

**Returns:**
boolean
### getInterruptMonitor() {#getInterruptMonitor--}
```
public AbstractInterruptMonitor getInterruptMonitor()
```


Gets the interrupt monitor.

**Returns:**
[AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
### getKeepPrecision() {#getKeepPrecision--}
```
public boolean getKeepPrecision()
```


Indicates whether not parsing a string value if the length is 15.

**Returns:**
boolean
### getKeepUnparsedData() {#getKeepUnparsedData--}
```
public boolean getKeepUnparsedData()
```


Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true.

**Remarks**

For scenarios that user only needs to read some contents from template file and does not need to save the workbook back, set this property as false may improve performance, especially when using it together with some kind of LoadFilter,

**Returns:**
boolean
### getLanguageCode() {#getLanguageCode--}
```
public int getLanguageCode()
```


Gets the user interface language of the Workbook version based on CountryCode that has saved the file.

See [CountryCode](../../com.aspose.cells/countrycode).

**Returns:**
int
### getLightCellsDataHandler() {#getLightCellsDataHandler--}
```
public LightCellsDataHandler getLightCellsDataHandler()
```


The data handler for processing cells data when reading template file.

**Returns:**
[LightCellsDataHandler](../../com.aspose.cells/lightcellsdatahandler)
### getLoadFilter() {#getLoadFilter--}
```
public LoadFilter getLoadFilter()
```


The filter to denote how to load data.

**Returns:**
[LoadFilter](../../com.aspose.cells/loadfilter)
### getLoadFormat() {#getLoadFormat--}
```
public int getLoadFormat()
```


Gets the load format.

See [LoadFormat](../../com.aspose.cells/loadformat).

**Returns:**
int
### getLoadFormulas() {#getLoadFormulas--}
```
public boolean getLoadFormulas()
```


Indicates whether importing formulas if the original html file contains formulas

**Returns:**
boolean
### getLoadStyleStrategy() {#getLoadStyleStrategy--}
```
public int getLoadStyleStrategy()
```


Indicates the strategy to apply style for parsed values when converting string value to number or datetime.

See [TxtLoadStyleStrategy](../../com.aspose.cells/txtloadstylestrategy).

**Returns:**
int
### getLocale() {#getLocale--}
```
public Locale getLocale()
```


Gets the regional settings used for the Workbook that will be loaded.

**Remarks**

This property has the same effect with [getRegion()](../../com.aspose.cells/loadoptions\#getRegion--) for setting regional settings.

**Returns:**
java.util.Locale
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


Gets the memory mode for loaded workbook.

See [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

For more details about memory mode, please see [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Returns:**
int
### getParsingFormulaOnOpen() {#getParsingFormulaOnOpen--}
```
public boolean getParsingFormulaOnOpen()
```


Indicates whether parsing the formula when reading the file.

**Remarks**

Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file because the formulas in the files are stored with a string formula.

**Returns:**
boolean
### getParsingPivotCachedRecords() {#getParsingPivotCachedRecords--}
```
public boolean getParsingPivotCachedRecords()
```


Indicates whether parsing pivot cached records when loading the file. The default value is false.

**Remarks**

Only applies for Excel Xlsx, Xltx, Xltm , Xlsm and xlsb file

**Returns:**
boolean
### getPassword() {#getPassword--}
```
public String getPassword()
```


Gets the password of the workbook.

**Returns:**
java.lang.String
### getPreservePaddingSpacesInFormula() {#getPreservePaddingSpacesInFormula--}
```
public boolean getPreservePaddingSpacesInFormula()
```


Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false.

**Remarks**

After loading workbook from template file with this option, [FormulaSettings.getPreservePaddingSpaces()](../../com.aspose.cells/formulasettings\#getPreservePaddingSpaces--) will be set to the same value with this property.

**Returns:**
boolean
### getProgId() {#getProgId--}
```
public String getProgId()
```


Gets the program id of creating the file. Only for MHT files.

**Returns:**
java.lang.String
### getRegion() {#getRegion--}
```
public int getRegion()
```


Gets the regional settings used for the Workbook that will be loaded.

See [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

The regional settings may be used for initializing some features for the workbook such as fonts, themes, and so on. For text based file formats, such as CSV, HTML, ..., the regional setting also will be used to detect number formats and parse text values to numeric or datetime values for cells. This setting will be kept for the instantiated workbook later, that is, [WorkbookSettings.getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) of the workbook will use the same region with this property.

**Returns:**
int
### getStandardFont() {#getStandardFont--}
```
public String getStandardFont()
```


Sets the default standard font name

**Remarks**

NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
java.lang.String
### getStandardFontSize() {#getStandardFontSize--}
```
public double getStandardFontSize()
```


Sets the default standard font size.

**Remarks**

NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
double
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


Gets the StreamProviderImportHtmlFile for importing objects.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getSupportDivTag() {#getSupportDivTag--}
```
public boolean getSupportDivTag()
```


Indicates whether support the layout of `<div>` tag when the html file contains it. The default value is false.

**Returns:**
boolean
### getTableLoadOptions() {#getTableLoadOptions--}
```
public HtmlTableLoadOptionCollection getTableLoadOptions()
```


Get the HtmlTableLoadOptionCollection instance

**Returns:**
[HtmlTableLoadOptionCollection](../../com.aspose.cells/htmltableloadoptioncollection)
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Gets warning callback.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### hasFormula() {#hasFormula--}
```
public boolean hasFormula()
```


Indicates whether the text is formula if it starts with "=".

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAttachedFilesDirectory(String value) {#setAttachedFilesDirectory-java.lang.String-}
```
public void setAttachedFilesDirectory(String value)
```


The directory that the attached files will be saved to.

**Remarks**

NOTE: This member is now obsolete. Instead, please use HtmlLoadOptions.StreamProvider property. This property will be removed 12 months later since December 2014. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setAutoFilter(boolean value) {#setAutoFilter-boolean-}
```
public void setAutoFilter(boolean value)
```


Indicates whether auto filtering the data when loading the files.

**Remarks**

Sometimes although autofilter is set, the corresponding rows is not hidden in the file. Now only works for SpreadSheetML file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutoFitColsAndRows(boolean value) {#setAutoFitColsAndRows-boolean-}
```
public void setAutoFitColsAndRows(boolean value)
```


Indicates whether auto-fit columns and rows. The default value is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutoFitterOptions(AutoFitterOptions value) {#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-}
```
public void setAutoFitterOptions(AutoFitterOptions value)
```


Sets the auto fitter options

**Remarks**

Only for xlsx ,spreadsheetML file now.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) |  |

### setCheckDataValid(boolean value) {#setCheckDataValid-boolean-}
```
public void setCheckDataValid(boolean value)
```


Check whether data is valid in the template file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setConvertDateTimeData(boolean value) {#setConvertDateTimeData-boolean-}
```
public void setConvertDateTimeData(boolean value)
```


Sets a value that indicates whether the string in text file is converted to date data. Default value is true.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setConvertFormulasData(boolean value) {#setConvertFormulasData-boolean-}
```
public void setConvertFormulasData(boolean value)
```


if true, convert string to formula when string value starts with character '=',the default value is false.

**Remarks**

NOTE: This property is now obsolete. Instead, please use HtmlLoadOptions.HasFormula property. This property will be removed 12 months later since March 2023. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Sets a value that indicates whether the string in text file is converted to numeric data. Default value is true.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDeleteRedundantSpaces(boolean value) {#setDeleteRedundantSpaces-boolean-}
```
public void setDeleteRedundantSpaces(boolean value)
```


Indicates whether delete redundant spaces when the text wraps lines using `<br>` tag. The default value is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Sets the default encoding. Only applies for csv file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setFontConfigs(IndividualFontConfigs value) {#setFontConfigs-com.aspose.cells.IndividualFontConfigs-}
```
public void setFontConfigs(IndividualFontConfigs value)
```


Sets individual font configs. Only works for the [Workbook](../../com.aspose.cells/workbook) which uses this [LoadOptions](../../com.aspose.cells/loadoptions) to load.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs) |  |

### setHasFormula(boolean value) {#setHasFormula-boolean-}
```
public void setHasFormula(boolean value)
```


Indicates whether the text is formula if it starts with "=".

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setIgnoreNotPrinted(boolean value) {#setIgnoreNotPrinted-boolean-}
```
public void setIgnoreNotPrinted(boolean value)
```


Ignore the data which are not printed if directly printing the file

**Remarks**

Only for xlsx file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setIgnoreUselessShapes(boolean value) {#setIgnoreUselessShapes-boolean-}
```
public void setIgnoreUselessShapes(boolean value)
```


Indicates whether ignoring useless shapes.

**Remarks**

Only works for xlsx,xlsb, and xlsm files. There are many overlapping identical shapes which are useless in some files, we can ingore them when loading files.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setInterruptMonitor(AbstractInterruptMonitor value) {#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-}
```
public void setInterruptMonitor(AbstractInterruptMonitor value)
```


Sets the interrupt monitor.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) |  |

### setKeepPrecision(boolean value) {#setKeepPrecision-boolean-}
```
public void setKeepPrecision(boolean value)
```


Indicates whether not parsing a string value if the length is 15.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setKeepUnparsedData(boolean value) {#setKeepUnparsedData-boolean-}
```
public void setKeepUnparsedData(boolean value)
```


Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true.

**Remarks**

For scenarios that user only needs to read some contents from template file and does not need to save the workbook back, set this property as false may improve performance, especially when using it together with some kind of LoadFilter,

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


Sets the user interface language of the Workbook version based on CountryCode that has saved the file.

See [CountryCode](../../com.aspose.cells/countrycode).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLightCellsDataHandler(LightCellsDataHandler value) {#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-}
```
public void setLightCellsDataHandler(LightCellsDataHandler value)
```


The data handler for processing cells data when reading template file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LightCellsDataHandler](../../com.aspose.cells/lightcellsdatahandler) |  |

### setLoadFilter(LoadFilter value) {#setLoadFilter-com.aspose.cells.LoadFilter-}
```
public void setLoadFilter(LoadFilter value)
```


The filter to denote how to load data.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LoadFilter](../../com.aspose.cells/loadfilter) |  |

### setLoadFormulas(boolean value) {#setLoadFormulas-boolean-}
```
public void setLoadFormulas(boolean value)
```


Indicates whether importing formulas if the original html file contains formulas

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setLoadStyleStrategy(int value) {#setLoadStyleStrategy-int-}
```
public void setLoadStyleStrategy(int value)
```


Indicates the strategy to apply style for parsed values when converting string value to number or datetime.

See [TxtLoadStyleStrategy](../../com.aspose.cells/txtloadstylestrategy).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLocale(Locale value) {#setLocale-java.util.Locale-}
```
public void setLocale(Locale value)
```


Sets the regional settings used for the Workbook that will be loaded.

**Remarks**

This property has the same effect with [getRegion()](../../com.aspose.cells/loadoptions\#getRegion--) for setting regional settings.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Locale |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


Sets the memory mode for loaded workbook.

See [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

For more details about memory mode, please see [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPaperSize(int type) {#setPaperSize-int-}
```
public void setPaperSize(int type)
```


Sets the default print paper size from default printer's setting.

**Remarks**

If there is no setting about paper size,MS Excel will use default printer's setting.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [PaperSizeType](../../com.aspose.cells/papersizetype). The default paper size. |

### setParsingFormulaOnOpen(boolean value) {#setParsingFormulaOnOpen-boolean-}
```
public void setParsingFormulaOnOpen(boolean value)
```


Indicates whether parsing the formula when reading the file.

**Remarks**

Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file because the formulas in the files are stored with a string formula.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setParsingPivotCachedRecords(boolean value) {#setParsingPivotCachedRecords-boolean-}
```
public void setParsingPivotCachedRecords(boolean value)
```


Indicates whether parsing pivot cached records when loading the file. The default value is false.

**Remarks**

Only applies for Excel Xlsx, Xltx, Xltm , Xlsm and xlsb file

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Sets the password of the workbook.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setPreservePaddingSpacesInFormula(boolean value) {#setPreservePaddingSpacesInFormula-boolean-}
```
public void setPreservePaddingSpacesInFormula(boolean value)
```


Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false.

**Remarks**

After loading workbook from template file with this option, [FormulaSettings.getPreservePaddingSpaces()](../../com.aspose.cells/formulasettings\#getPreservePaddingSpaces--) will be set to the same value with this property.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setRegion(int value) {#setRegion-int-}
```
public void setRegion(int value)
```


Sets the regional settings used for the Workbook that will be loaded.

See [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

The regional settings may be used for initializing some features for the workbook such as fonts, themes, and so on. For text based file formats, such as CSV, HTML, ..., the regional setting also will be used to detect number formats and parse text values to numeric or datetime values for cells. This setting will be kept for the instantiated workbook later, that is, [WorkbookSettings.getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) of the workbook will use the same region with this property.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setStandardFont(String value) {#setStandardFont-java.lang.String-}
```
public void setStandardFont(String value)
```


Sets the default standard font name

**Remarks**

NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setStandardFontSize(double value) {#setStandardFontSize-double-}
```
public void setStandardFontSize(double value)
```


Sets the default standard font size.

**Remarks**

NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


Sets the StreamProviderImportHtmlFile for importing objects.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setSupportDivTag(boolean value) {#setSupportDivTag-boolean-}
```
public void setSupportDivTag(boolean value)
```


Indicates whether support the layout of `<div>` tag when the html file contains it. The default value is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


Sets warning callback.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

