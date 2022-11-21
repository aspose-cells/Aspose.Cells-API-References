---
title: HtmlLoadOptions
second_title: Aspose.Cells for Java API Reference
description: Represents options when importing a html file.
type: docs
weight: 264
url: /java/com.aspose.cells/htmlloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LoadOptions](../../com.aspose.cells/loadoptions), [com.aspose.cells.AbstractTextLoadOptions](../../com.aspose.cells/abstracttextloadoptions)
```
public class HtmlLoadOptions extends AbstractTextLoadOptions
```

Represents options when importing a html file.
## Constructors

| Constructor | Description |
| --- | --- |
| [HtmlLoadOptions()](#HtmlLoadOptions--) | Creates an options of loading the file. |
| [HtmlLoadOptions(int loadFormat)](#HtmlLoadOptions-int-) | Creates an options of loading the file. |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--) | The directory that the attached files will be saved to. |
| [getAutoFilter()](#getAutoFilter--) | Indicates whether auto filtering the data when loading the files. |
| [getAutoFitColsAndRows()](#getAutoFitColsAndRows--) | Indicates whether auto-fit columns and rows. |
| [getAutoFitterOptions()](#getAutoFitterOptions--) | Gets and sets the auto fitter options Only for xlsx ,spreadsheetML file now. |
| [getCheckDataValid()](#getCheckDataValid--) | Check whether data is valid in the template file. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Whether check restriction of excel file when user modify cells related objects. |
| [getClass()](#getClass--) |  |
| [getConvertDateTimeData()](#getConvertDateTimeData--) | Gets or sets a value that indicates whether the string in text file is converted to date data. |
| [getConvertFormulasData()](#getConvertFormulasData--) | if true, convert string to formula when string value starts with character '=',the default value is false. |
| [getConvertNumericData()](#getConvertNumericData--) | Gets or sets a value that indicates whether the string in text file is converted to numeric data. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Gets the default style settings for initializing styles of the workbook |
| [getDeleteRedundantSpaces()](#getDeleteRedundantSpaces--) | Indicates whether delete redundant spaces when the text wraps lines using <br>tag.The default value is false. |
| [getEncoding()](#getEncoding--) | Gets and sets the default encoding. |
| [getFontConfigs()](#getFontConfigs--) | Gets and sets individual font configs. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Ignore the data which are not printed if directly printing the file Only for xlsx file. |
| [getInterruptMonitor()](#getInterruptMonitor--) | Gets and sets the interrupt monitor. |
| [getKeepPrecision()](#getKeepPrecision--) | Indicates whether not parsing a string value if the length is 15. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. |
| [getLanguageCode()](#getLanguageCode--) | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [getLightCellsDataHandler()](#getLightCellsDataHandler--) | The data handler for processing cells data when reading template file. |
| [getLoadFilter()](#getLoadFilter--) | The filter to denote how to load data. |
| [getLoadFormat()](#getLoadFormat--) | Gets the load format. |
| [getLoadFormulas()](#getLoadFormulas--) | Indicates whether importing formulas if the original html file contains formulas |
| [getLoadStyleStrategy()](#getLoadStyleStrategy--) | Indicates the strategy to apply style for parsed values when converting string value to number or datetime. |
| [getLocale()](#getLocale--) | Gets and sets the Locale used for workbook at the time the file was loaded. |
| [getMemorySetting()](#getMemorySetting--) | Gets or sets the memory usage options. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Indicates whether parsing the formula when reading the file. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Indicates whether parsing pivot cached records when loading the file. |
| [getPassword()](#getPassword--) | Gets and set the password of the workbook. |
| [getProgId()](#getProgId--) | Gets the program id of creating the file. |
| [getRegion()](#getRegion--) | Gets or sets the system regional settings based on CountryCode at the time the file was loaded. |
| [getStandardFont()](#getStandardFont--) | Sets the default standard font name NOTE: This member is now obsolete. |
| [getStandardFontSize()](#getStandardFontSize--) | Sets the default standard font size. |
| [getStreamProvider()](#getStreamProvider--) | Gets or sets the StreamProviderImportHtmlFile for importing objects. |
| [getSupportDivTag()](#getSupportDivTag--) | Indicates whether support the layout of <div> tag when the html file contains <div> tags. |
| [getWarningCallback()](#getWarningCallback--) | Gets or sets warning callback. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | For the description of this property, please see [getAttachedFilesDirectory()](../../com.aspose.cells/htmlloadoptions\#getAttachedFilesDirectory--) |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | For the description of this property, please see [getAutoFilter()](../../com.aspose.cells/loadoptions\#getAutoFilter--) |
| [setAutoFitColsAndRows(boolean value)](#setAutoFitColsAndRows-boolean-) | For the description of this property, please see [getAutoFitColsAndRows()](../../com.aspose.cells/htmlloadoptions\#getAutoFitColsAndRows--) |
| [setAutoFitterOptions(AutoFitterOptions value)](#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-) | For the description of this property, please see [getAutoFitterOptions()](../../com.aspose.cells/loadoptions\#getAutoFitterOptions--) |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | For the description of this property, please see [getCheckDataValid()](../../com.aspose.cells/loadoptions\#getCheckDataValid--) |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | For the description of this property, please see [getCheckExcelRestriction()](../../com.aspose.cells/loadoptions\#getCheckExcelRestriction--) |
| [setConvertDateTimeData(boolean value)](#setConvertDateTimeData-boolean-) | For the description of this property, please see [getConvertDateTimeData()](../../com.aspose.cells/abstracttextloadoptions\#getConvertDateTimeData--) |
| [setConvertFormulasData(boolean value)](#setConvertFormulasData-boolean-) | For the description of this property, please see [getConvertFormulasData()](../../com.aspose.cells/htmlloadoptions\#getConvertFormulasData--) |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | For the description of this property, please see [getConvertNumericData()](../../com.aspose.cells/abstracttextloadoptions\#getConvertNumericData--) |
| [setDeleteRedundantSpaces(boolean value)](#setDeleteRedundantSpaces-boolean-) | For the description of this property, please see [getDeleteRedundantSpaces()](../../com.aspose.cells/htmlloadoptions\#getDeleteRedundantSpaces--) |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | For the description of this property, please see [getEncoding()](../../com.aspose.cells/abstracttextloadoptions\#getEncoding--) |
| [setFontConfigs(IndividualFontConfigs value)](#setFontConfigs-com.aspose.cells.IndividualFontConfigs-) | For the description of this property, please see [getFontConfigs()](../../com.aspose.cells/loadoptions\#getFontConfigs--) |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | For the description of this property, please see [getIgnoreNotPrinted()](../../com.aspose.cells/loadoptions\#getIgnoreNotPrinted--) |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | For the description of this property, please see [getInterruptMonitor()](../../com.aspose.cells/loadoptions\#getInterruptMonitor--) |
| [setKeepPrecision(boolean value)](#setKeepPrecision-boolean-) | For the description of this property, please see [getKeepPrecision()](../../com.aspose.cells/abstracttextloadoptions\#getKeepPrecision--) |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | For the description of this property, please see [getKeepUnparsedData()](../../com.aspose.cells/loadoptions\#getKeepUnparsedData--) |
| [setLanguageCode(int value)](#setLanguageCode-int-) | For the description of this property, please see [getLanguageCode()](../../com.aspose.cells/loadoptions\#getLanguageCode--) |
| [setLightCellsDataHandler(LightCellsDataHandler value)](#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-) | For the description of this property, please see [getLightCellsDataHandler()](../../com.aspose.cells/loadoptions\#getLightCellsDataHandler--) |
| [setLoadFilter(LoadFilter value)](#setLoadFilter-com.aspose.cells.LoadFilter-) | For the description of this property, please see [getLoadFilter()](../../com.aspose.cells/loadoptions\#getLoadFilter--) |
| [setLoadFormulas(boolean value)](#setLoadFormulas-boolean-) | For the description of this property, please see [getLoadFormulas()](../../com.aspose.cells/htmlloadoptions\#getLoadFormulas--) |
| [setLoadStyleStrategy(int value)](#setLoadStyleStrategy-int-) | For the description of this property, please see [getLoadStyleStrategy()](../../com.aspose.cells/abstracttextloadoptions\#getLoadStyleStrategy--) |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | For the description of this property, please see [getLocale()](../../com.aspose.cells/loadoptions\#getLocale--) |
| [setMemorySetting(int value)](#setMemorySetting-int-) | For the description of this property, please see [getMemorySetting()](../../com.aspose.cells/loadoptions\#getMemorySetting--) |
| [setPaperSize(int type)](#setPaperSize-int-) | Sets the default print paper size from default printer's setting. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | For the description of this property, please see [getParsingFormulaOnOpen()](../../com.aspose.cells/loadoptions\#getParsingFormulaOnOpen--) |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | For the description of this property, please see [getParsingPivotCachedRecords()](../../com.aspose.cells/loadoptions\#getParsingPivotCachedRecords--) |
| [setPassword(String value)](#setPassword-java.lang.String-) | For the description of this property, please see [getPassword()](../../com.aspose.cells/loadoptions\#getPassword--) |
| [setRegion(int value)](#setRegion-int-) | For the description of this property, please see [getRegion()](../../com.aspose.cells/loadoptions\#getRegion--) |
| [setStandardFont(String value)](#setStandardFont-java.lang.String-) | For the description of this property, please see [getStandardFont()](../../com.aspose.cells/loadoptions\#getStandardFont--) |
| [setStandardFontSize(double value)](#setStandardFontSize-double-) | For the description of this property, please see [getStandardFontSize()](../../com.aspose.cells/loadoptions\#getStandardFontSize--) |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | For the description of this property, please see [getStreamProvider()](../../com.aspose.cells/htmlloadoptions\#getStreamProvider--) |
| [setSupportDivTag(boolean value)](#setSupportDivTag-boolean-) | For the description of this property, please see [getSupportDivTag()](../../com.aspose.cells/htmlloadoptions\#getSupportDivTag--) |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### HtmlLoadOptions() {#HtmlLoadOptions--}
```
public HtmlLoadOptions()
```


Creates an options of loading the file.

### HtmlLoadOptions(int loadFormat) {#HtmlLoadOptions-int-}
```
public HtmlLoadOptions(int loadFormat)
```


Creates an options of loading the file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | int | The loading format. |

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


The directory that the attached files will be saved to. NOTE: This member is now obsolete. Instead, please use HtmlLoadOptions.StreamProvider property. This property will be removed 12 months later since December 2014. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
java.lang.String
### getAutoFilter() {#getAutoFilter--}
```
public boolean getAutoFilter()
```


Indicates whether auto filtering the data when loading the files. Sometimes although autofilter is set, the corresponding rows is not hidden in the file. Now only works for SpreadSheetML file.

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


Gets and sets the auto fitter options Only for xlsx ,spreadsheetML file now.

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


Gets or sets a value that indicates whether the string in text file is converted to date data.

**Returns:**
boolean
### getConvertFormulasData() {#getConvertFormulasData--}
```
public boolean getConvertFormulasData()
```


if true, convert string to formula when string value starts with character '=',the default value is false.

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Gets or sets a value that indicates whether the string in text file is converted to numeric data.

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


Indicates whether delete redundant spaces when the text wraps lines using <br>tag.The default value is false.

**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Gets and sets the default encoding. Only applies for csv file.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getFontConfigs() {#getFontConfigs--}
```
public IndividualFontConfigs getFontConfigs()
```


Gets and sets individual font configs. Only works for the [Workbook](../../com.aspose.cells/workbook) which uses this [LoadOptions](../../com.aspose.cells/loadoptions) to load.

**Returns:**
[IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs)
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```


Ignore the data which are not printed if directly printing the file Only for xlsx file.

**Returns:**
boolean
### getInterruptMonitor() {#getInterruptMonitor--}
```
public AbstractInterruptMonitor getInterruptMonitor()
```


Gets and sets the interrupt monitor.

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


Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. For scenarios that user only needs to read some contents from template file and does not need to save the workbook back, set this property as false may improve performance, especially when using it together with some kind of LoadFilter,

**Returns:**
boolean
### getLanguageCode() {#getLanguageCode--}
```
public int getLanguageCode()
```


Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file.

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

**Returns:**
int
### getLocale() {#getLocale--}
```
public Locale getLocale()
```


Gets and sets the Locale used for workbook at the time the file was loaded.

**Returns:**
java.util.Locale
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


Gets or sets the memory usage options.

**Returns:**
int
### getParsingFormulaOnOpen() {#getParsingFormulaOnOpen--}
```
public boolean getParsingFormulaOnOpen()
```


Indicates whether parsing the formula when reading the file. Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file because the formulas in the files are stored with a string formula.

**Returns:**
boolean
### getParsingPivotCachedRecords() {#getParsingPivotCachedRecords--}
```
public boolean getParsingPivotCachedRecords()
```


Indicates whether parsing pivot cached records when loading the file. The default value is false. Only applies for Excel Xlsx, Xltx, Xltm , Xlsm and xlsb file

**Returns:**
boolean
### getPassword() {#getPassword--}
```
public String getPassword()
```


Gets and set the password of the workbook.

**Returns:**
java.lang.String
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


Gets or sets the system regional settings based on CountryCode at the time the file was loaded. If you do not want to use the region saved in the file, please reset it after reading the file.

**Returns:**
int
### getStandardFont() {#getStandardFont--}
```
public String getStandardFont()
```


Sets the default standard font name NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
java.lang.String
### getStandardFontSize() {#getStandardFontSize--}
```
public double getStandardFontSize()
```


Sets the default standard font size. NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
double
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


Gets or sets the StreamProviderImportHtmlFile for importing objects.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getSupportDivTag() {#getSupportDivTag--}
```
public boolean getSupportDivTag()
```


Indicates whether support the layout of <div> tag when the html file contains <div> tags. The default value is false.

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Gets or sets warning callback.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
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


For the description of this property, please see [getAttachedFilesDirectory()](../../com.aspose.cells/htmlloadoptions\#getAttachedFilesDirectory--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setAutoFilter(boolean value) {#setAutoFilter-boolean-}
```
public void setAutoFilter(boolean value)
```


For the description of this property, please see [getAutoFilter()](../../com.aspose.cells/loadoptions\#getAutoFilter--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutoFitColsAndRows(boolean value) {#setAutoFitColsAndRows-boolean-}
```
public void setAutoFitColsAndRows(boolean value)
```


For the description of this property, please see [getAutoFitColsAndRows()](../../com.aspose.cells/htmlloadoptions\#getAutoFitColsAndRows--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutoFitterOptions(AutoFitterOptions value) {#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-}
```
public void setAutoFitterOptions(AutoFitterOptions value)
```


For the description of this property, please see [getAutoFitterOptions()](../../com.aspose.cells/loadoptions\#getAutoFitterOptions--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) |  |

### setCheckDataValid(boolean value) {#setCheckDataValid-boolean-}
```
public void setCheckDataValid(boolean value)
```


For the description of this property, please see [getCheckDataValid()](../../com.aspose.cells/loadoptions\#getCheckDataValid--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


For the description of this property, please see [getCheckExcelRestriction()](../../com.aspose.cells/loadoptions\#getCheckExcelRestriction--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setConvertDateTimeData(boolean value) {#setConvertDateTimeData-boolean-}
```
public void setConvertDateTimeData(boolean value)
```


For the description of this property, please see [getConvertDateTimeData()](../../com.aspose.cells/abstracttextloadoptions\#getConvertDateTimeData--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setConvertFormulasData(boolean value) {#setConvertFormulasData-boolean-}
```
public void setConvertFormulasData(boolean value)
```


For the description of this property, please see [getConvertFormulasData()](../../com.aspose.cells/htmlloadoptions\#getConvertFormulasData--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


For the description of this property, please see [getConvertNumericData()](../../com.aspose.cells/abstracttextloadoptions\#getConvertNumericData--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDeleteRedundantSpaces(boolean value) {#setDeleteRedundantSpaces-boolean-}
```
public void setDeleteRedundantSpaces(boolean value)
```


For the description of this property, please see [getDeleteRedundantSpaces()](../../com.aspose.cells/htmlloadoptions\#getDeleteRedundantSpaces--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


For the description of this property, please see [getEncoding()](../../com.aspose.cells/abstracttextloadoptions\#getEncoding--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setFontConfigs(IndividualFontConfigs value) {#setFontConfigs-com.aspose.cells.IndividualFontConfigs-}
```
public void setFontConfigs(IndividualFontConfigs value)
```


For the description of this property, please see [getFontConfigs()](../../com.aspose.cells/loadoptions\#getFontConfigs--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs) |  |

### setIgnoreNotPrinted(boolean value) {#setIgnoreNotPrinted-boolean-}
```
public void setIgnoreNotPrinted(boolean value)
```


For the description of this property, please see [getIgnoreNotPrinted()](../../com.aspose.cells/loadoptions\#getIgnoreNotPrinted--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setInterruptMonitor(AbstractInterruptMonitor value) {#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-}
```
public void setInterruptMonitor(AbstractInterruptMonitor value)
```


For the description of this property, please see [getInterruptMonitor()](../../com.aspose.cells/loadoptions\#getInterruptMonitor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) |  |

### setKeepPrecision(boolean value) {#setKeepPrecision-boolean-}
```
public void setKeepPrecision(boolean value)
```


For the description of this property, please see [getKeepPrecision()](../../com.aspose.cells/abstracttextloadoptions\#getKeepPrecision--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setKeepUnparsedData(boolean value) {#setKeepUnparsedData-boolean-}
```
public void setKeepUnparsedData(boolean value)
```


For the description of this property, please see [getKeepUnparsedData()](../../com.aspose.cells/loadoptions\#getKeepUnparsedData--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


For the description of this property, please see [getLanguageCode()](../../com.aspose.cells/loadoptions\#getLanguageCode--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLightCellsDataHandler(LightCellsDataHandler value) {#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-}
```
public void setLightCellsDataHandler(LightCellsDataHandler value)
```


For the description of this property, please see [getLightCellsDataHandler()](../../com.aspose.cells/loadoptions\#getLightCellsDataHandler--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LightCellsDataHandler](../../com.aspose.cells/lightcellsdatahandler) |  |

### setLoadFilter(LoadFilter value) {#setLoadFilter-com.aspose.cells.LoadFilter-}
```
public void setLoadFilter(LoadFilter value)
```


For the description of this property, please see [getLoadFilter()](../../com.aspose.cells/loadoptions\#getLoadFilter--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LoadFilter](../../com.aspose.cells/loadfilter) |  |

### setLoadFormulas(boolean value) {#setLoadFormulas-boolean-}
```
public void setLoadFormulas(boolean value)
```


For the description of this property, please see [getLoadFormulas()](../../com.aspose.cells/htmlloadoptions\#getLoadFormulas--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setLoadStyleStrategy(int value) {#setLoadStyleStrategy-int-}
```
public void setLoadStyleStrategy(int value)
```


For the description of this property, please see [getLoadStyleStrategy()](../../com.aspose.cells/abstracttextloadoptions\#getLoadStyleStrategy--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLocale(Locale value) {#setLocale-java.util.Locale-}
```
public void setLocale(Locale value)
```


For the description of this property, please see [getLocale()](../../com.aspose.cells/loadoptions\#getLocale--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Locale |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


For the description of this property, please see [getMemorySetting()](../../com.aspose.cells/loadoptions\#getMemorySetting--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPaperSize(int type) {#setPaperSize-int-}
```
public void setPaperSize(int type)
```


Sets the default print paper size from default printer's setting. If there is no setting about paper size,MS Excel will use default printer's setting.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | The default paper size. |

### setParsingFormulaOnOpen(boolean value) {#setParsingFormulaOnOpen-boolean-}
```
public void setParsingFormulaOnOpen(boolean value)
```


For the description of this property, please see [getParsingFormulaOnOpen()](../../com.aspose.cells/loadoptions\#getParsingFormulaOnOpen--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setParsingPivotCachedRecords(boolean value) {#setParsingPivotCachedRecords-boolean-}
```
public void setParsingPivotCachedRecords(boolean value)
```


For the description of this property, please see [getParsingPivotCachedRecords()](../../com.aspose.cells/loadoptions\#getParsingPivotCachedRecords--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


For the description of this property, please see [getPassword()](../../com.aspose.cells/loadoptions\#getPassword--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setRegion(int value) {#setRegion-int-}
```
public void setRegion(int value)
```


For the description of this property, please see [getRegion()](../../com.aspose.cells/loadoptions\#getRegion--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setStandardFont(String value) {#setStandardFont-java.lang.String-}
```
public void setStandardFont(String value)
```


For the description of this property, please see [getStandardFont()](../../com.aspose.cells/loadoptions\#getStandardFont--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setStandardFontSize(double value) {#setStandardFontSize-double-}
```
public void setStandardFontSize(double value)
```


For the description of this property, please see [getStandardFontSize()](../../com.aspose.cells/loadoptions\#getStandardFontSize--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


For the description of this property, please see [getStreamProvider()](../../com.aspose.cells/htmlloadoptions\#getStreamProvider--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setSupportDivTag(boolean value) {#setSupportDivTag-boolean-}
```
public void setSupportDivTag(boolean value)
```


For the description of this property, please see [getSupportDivTag()](../../com.aspose.cells/htmlloadoptions\#getSupportDivTag--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```




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

