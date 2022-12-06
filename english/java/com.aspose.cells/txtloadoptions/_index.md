---
title: TxtLoadOptions
second_title: Aspose.Cells for Java API Reference
description: Represents the options for loading text file.
type: docs
url: /java/com.aspose.cells/txtloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LoadOptions](../../com.aspose.cells/loadoptions), [com.aspose.cells.AbstractTextLoadOptions](../../com.aspose.cells/abstracttextloadoptions)
```
public class TxtLoadOptions extends AbstractTextLoadOptions
```

Represents the options for loading text file.
## Constructors

| Constructor | Description |
| --- | --- |
| [TxtLoadOptions()](#TxtLoadOptions--) | Creates the options for loading text file. |
| [TxtLoadOptions(int loadFormat)](#TxtLoadOptions-int-) | Creates the options for loading text file. |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Indicates whether auto filtering the data when loading the files. |
| [getAutoFitterOptions()](#getAutoFitterOptions--) | the auto fitter options Only for xlsx ,spreadsheetML file now. |
| [getCheckDataValid()](#getCheckDataValid--) | Check whether data is valid in the template file. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Whether check restriction of excel file when user modify cells related objects. |
| [getClass()](#getClass--) |  |
| [getConvertDateTimeData()](#getConvertDateTimeData--) | a value that indicates whether the string in text file is converted to date data. |
| [getConvertNumericData()](#getConvertNumericData--) | a value that indicates whether the string in text file is converted to numeric data. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Gets the default style settings for initializing styles of the workbook |
| [getEncoding()](#getEncoding--) | the default encoding. |
| [getExtendToNextSheet()](#getExtendToNextSheet--) | Whether extends data to next sheet when the rows or columns of data exceed limit. |
| [getFontConfigs()](#getFontConfigs--) | individual font configs. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Ignore the data which are not printed if directly printing the file Only for xlsx file. |
| [getInterruptMonitor()](#getInterruptMonitor--) | the interrupt monitor. |
| [getKeepPrecision()](#getKeepPrecision--) | Indicates whether not parsing a string value if the length is 15. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. |
| [getLanguageCode()](#getLanguageCode--) | the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [getLightCellsDataHandler()](#getLightCellsDataHandler--) | The data handler for processing cells data when reading template file. |
| [getLoadFilter()](#getLoadFilter--) | The filter to denote how to load data. |
| [getLoadFormat()](#getLoadFormat--) | Gets the load format. |
| [getLoadStyleStrategy()](#getLoadStyleStrategy--) | Indicates the strategy to apply style for parsed values when converting string value to number or datetime. |
| [getLocale()](#getLocale--) | the Locale used for workbook at the time the file was loaded. |
| [getMemorySetting()](#getMemorySetting--) | the memory usage options. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Indicates whether parsing the formula when reading the file. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Indicates whether parsing pivot cached records when loading the file. |
| [getPassword()](#getPassword--) | the password of the workbook. |
| [getPreferredParsers()](#getPreferredParsers--) | preferred value parsers for loading text file. |
| [getRegion()](#getRegion--) | the system regional settings based on CountryCode at the time the file was loaded. |
| [getSeparator()](#getSeparator--) | character separator of text file. |
| [getSeparatorString()](#getSeparatorString--) | a string value as separator. |
| [getStandardFont()](#getStandardFont--) | Sets the default standard font name NOTE: This member is now obsolete. |
| [getStandardFontSize()](#getStandardFontSize--) | Sets the default standard font size. |
| [getTextQualifier()](#getTextQualifier--) | Specifies the text qualifier for cell values. |
| [getTreatConsecutiveDelimitersAsOne()](#getTreatConsecutiveDelimitersAsOne--) | Whether consecutive delimiters should be treated as one. |
| [getTreatQuotePrefixAsValue()](#getTreatQuotePrefixAsValue--) | Indicates whether the leading single quote sign should be taken as part of the value of one cell. |
| [getWarningCallback()](#getWarningCallback--) | warning callback. |
| [hasFormula()](#hasFormula--) | Indicates whether the text is formula if it starts with "=". |
| [hasTextQualifier()](#hasTextQualifier--) | Whether there is text qualifier for cell value. |
| [hashCode()](#hashCode--) |  |
| [isMultiEncoded()](#isMultiEncoded--) | True means that the file contains several encoding. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | For the description of this property, please see [getAutoFilter()](../../com.aspose.cells/loadoptions\#getAutoFilter--) |
| [setAutoFitterOptions(AutoFitterOptions value)](#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-) | For the description of this property, please see [getAutoFitterOptions()](../../com.aspose.cells/loadoptions\#getAutoFitterOptions--) |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | For the description of this property, please see [getCheckDataValid()](../../com.aspose.cells/loadoptions\#getCheckDataValid--) |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | For the description of this property, please see [getCheckExcelRestriction()](../../com.aspose.cells/loadoptions\#getCheckExcelRestriction--) |
| [setConvertDateTimeData(boolean value)](#setConvertDateTimeData-boolean-) | For the description of this property, please see [getConvertDateTimeData()](../../com.aspose.cells/abstracttextloadoptions\#getConvertDateTimeData--) |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | For the description of this property, please see [getConvertNumericData()](../../com.aspose.cells/abstracttextloadoptions\#getConvertNumericData--) |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | For the description of this property, please see [getEncoding()](../../com.aspose.cells/abstracttextloadoptions\#getEncoding--) |
| [setExtendToNextSheet(boolean value)](#setExtendToNextSheet-boolean-) | For the description of this property, please see [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--) |
| [setFontConfigs(IndividualFontConfigs value)](#setFontConfigs-com.aspose.cells.IndividualFontConfigs-) | For the description of this property, please see [getFontConfigs()](../../com.aspose.cells/loadoptions\#getFontConfigs--) |
| [setHasFormula(boolean value)](#setHasFormula-boolean-) | For the description of this property, please see [hasFormula()](../../com.aspose.cells/txtloadoptions\#hasFormula--) |
| [setHasTextQualifier(boolean value)](#setHasTextQualifier-boolean-) | For the description of this property, please see [hasTextQualifier()](../../com.aspose.cells/txtloadoptions\#hasTextQualifier--) |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | For the description of this property, please see [getIgnoreNotPrinted()](../../com.aspose.cells/loadoptions\#getIgnoreNotPrinted--) |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | For the description of this property, please see [getInterruptMonitor()](../../com.aspose.cells/loadoptions\#getInterruptMonitor--) |
| [setKeepPrecision(boolean value)](#setKeepPrecision-boolean-) | For the description of this property, please see [getKeepPrecision()](../../com.aspose.cells/abstracttextloadoptions\#getKeepPrecision--) |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | For the description of this property, please see [getKeepUnparsedData()](../../com.aspose.cells/loadoptions\#getKeepUnparsedData--) |
| [setLanguageCode(int value)](#setLanguageCode-int-) | For the description of this property, please see [getLanguageCode()](../../com.aspose.cells/loadoptions\#getLanguageCode--) |
| [setLightCellsDataHandler(LightCellsDataHandler value)](#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-) | For the description of this property, please see [getLightCellsDataHandler()](../../com.aspose.cells/loadoptions\#getLightCellsDataHandler--) |
| [setLoadFilter(LoadFilter value)](#setLoadFilter-com.aspose.cells.LoadFilter-) | For the description of this property, please see [getLoadFilter()](../../com.aspose.cells/loadoptions\#getLoadFilter--) |
| [setLoadStyleStrategy(int value)](#setLoadStyleStrategy-int-) | For the description of this property, please see [getLoadStyleStrategy()](../../com.aspose.cells/abstracttextloadoptions\#getLoadStyleStrategy--) |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | For the description of this property, please see [getLocale()](../../com.aspose.cells/loadoptions\#getLocale--) |
| [setMemorySetting(int value)](#setMemorySetting-int-) | For the description of this property, please see [getMemorySetting()](../../com.aspose.cells/loadoptions\#getMemorySetting--) |
| [setMultiEncoded(boolean value)](#setMultiEncoded-boolean-) | For the description of this property, please see [isMultiEncoded()](../../com.aspose.cells/txtloadoptions\#isMultiEncoded--) |
| [setPaperSize(int type)](#setPaperSize-int-) | Sets the default print paper size from default printer's setting. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | For the description of this property, please see [getParsingFormulaOnOpen()](../../com.aspose.cells/loadoptions\#getParsingFormulaOnOpen--) |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | For the description of this property, please see [getParsingPivotCachedRecords()](../../com.aspose.cells/loadoptions\#getParsingPivotCachedRecords--) |
| [setPassword(String value)](#setPassword-java.lang.String-) | For the description of this property, please see [getPassword()](../../com.aspose.cells/loadoptions\#getPassword--) |
| [setPreferredParsers(ICustomParser[] value)](#setPreferredParsers-com.aspose.cells.ICustomParser---) | For the description of this property, please see [getPreferredParsers()](../../com.aspose.cells/txtloadoptions\#getPreferredParsers--) |
| [setRegion(int value)](#setRegion-int-) | For the description of this property, please see [getRegion()](../../com.aspose.cells/loadoptions\#getRegion--) |
| [setSeparator(char value)](#setSeparator-char-) | For the description of this property, please see [getSeparator()](../../com.aspose.cells/txtloadoptions\#getSeparator--) |
| [setSeparatorString(String value)](#setSeparatorString-java.lang.String-) | For the description of this property, please see [getSeparatorString()](../../com.aspose.cells/txtloadoptions\#getSeparatorString--) |
| [setStandardFont(String value)](#setStandardFont-java.lang.String-) | For the description of this property, please see [getStandardFont()](../../com.aspose.cells/loadoptions\#getStandardFont--) |
| [setStandardFontSize(double value)](#setStandardFontSize-double-) | For the description of this property, please see [getStandardFontSize()](../../com.aspose.cells/loadoptions\#getStandardFontSize--) |
| [setTextQualifier(char value)](#setTextQualifier-char-) | For the description of this property, please see [getTextQualifier()](../../com.aspose.cells/txtloadoptions\#getTextQualifier--) |
| [setTreatConsecutiveDelimitersAsOne(boolean value)](#setTreatConsecutiveDelimitersAsOne-boolean-) | For the description of this property, please see [getTreatConsecutiveDelimitersAsOne()](../../com.aspose.cells/txtloadoptions\#getTreatConsecutiveDelimitersAsOne--) |
| [setTreatQuotePrefixAsValue(boolean value)](#setTreatQuotePrefixAsValue-boolean-) | For the description of this property, please see [getTreatQuotePrefixAsValue()](../../com.aspose.cells/txtloadoptions\#getTreatQuotePrefixAsValue--) |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### TxtLoadOptions() {#TxtLoadOptions--}
```
public TxtLoadOptions()
```


Creates the options for loading text file. The default load file type is CSV .

### TxtLoadOptions(int loadFormat) {#TxtLoadOptions-int-}
```
public TxtLoadOptions(int loadFormat)
```


Creates the options for loading text file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | int | The loading format |

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
### getAutoFilter() {#getAutoFilter--}
```
public boolean getAutoFilter()
```


Indicates whether auto filtering the data when loading the files. Sometimes although autofilter is set, the corresponding rows is not hidden in the file. Now only works for SpreadSheetML file.

**Returns:**
boolean
### getAutoFitterOptions() {#getAutoFitterOptions--}
```
public AutoFitterOptions getAutoFitterOptions()
```


the auto fitter options Only for xlsx ,spreadsheetML file now.

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


a value that indicates whether the string in text file is converted to date data.

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


a value that indicates whether the string in text file is converted to numeric data.

**Returns:**
boolean
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```
public DefaultStyleSettings getDefaultStyleSettings()
```


Gets the default style settings for initializing styles of the workbook

**Returns:**
[DefaultStyleSettings](../../com.aspose.cells/defaultstylesettings)
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


the default encoding. Only applies for csv file.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getExtendToNextSheet() {#getExtendToNextSheet--}
```
public boolean getExtendToNextSheet()
```


Whether extends data to next sheet when the rows or columns of data exceed limit. If this property is true, extra data will be extended to next sheet behind current one(if current sheet is the last one, new sheet will be appended to current workbook). If this property is false, the data exceeds limit will be ignored. Default is false;

**Returns:**
boolean
### getFontConfigs() {#getFontConfigs--}
```
public IndividualFontConfigs getFontConfigs()
```


individual font configs. Only works for the [Workbook](../../com.aspose.cells/workbook) which uses this [LoadOptions](../../com.aspose.cells/loadoptions) to load.

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


the interrupt monitor.

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


the user interface language of the Workbook version based on CountryCode that has saved the file.

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


the Locale used for workbook at the time the file was loaded.

**Returns:**
java.util.Locale
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


the memory usage options.

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


the password of the workbook.

**Returns:**
java.lang.String
### getPreferredParsers() {#getPreferredParsers--}
```
public ICustomParser[] getPreferredParsers()
```


preferred value parsers for loading text file. parsers[0] is the parser will be used for the first column in text template file, parsers[1] is the parser will be used for the second column, ...etc. The last one(parsers[parsers.length-1]) will be used for all other columns start from parsers.length-1. If one item is null, the corresponding column will be parsed by the default parser of Aspose.Cells.

**Returns:**
com.aspose.cells.ICustomParser[]
### getRegion() {#getRegion--}
```
public int getRegion()
```


the system regional settings based on CountryCode at the time the file was loaded. If you do not want to use the region saved in the file, please reset it after reading the file.

**Returns:**
int
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```


character separator of text file.

**Returns:**
char
### getSeparatorString() {#getSeparatorString--}
```
public String getSeparatorString()
```


a string value as separator.

**Returns:**
java.lang.String
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
### getTextQualifier() {#getTextQualifier--}
```
public char getTextQualifier()
```


Specifies the text qualifier for cell values. Default qualifier is '"'. When setting this property, [hasTextQualifier()](../../com.aspose.cells/txtloadoptions\#hasTextQualifier--) will become true automatically.

**Returns:**
char
### getTreatConsecutiveDelimitersAsOne() {#getTreatConsecutiveDelimitersAsOne--}
```
public boolean getTreatConsecutiveDelimitersAsOne()
```


Whether consecutive delimiters should be treated as one.

**Returns:**
boolean
### getTreatQuotePrefixAsValue() {#getTreatQuotePrefixAsValue--}
```
public boolean getTreatQuotePrefixAsValue()
```


Indicates whether the leading single quote sign should be taken as part of the value of one cell. Default is true. If it is false, the leading single quote will be removed from corresponding cell's value and [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) will be set as true for the cell.

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


warning callback.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### hasFormula() {#hasFormula--}
```
public boolean hasFormula()
```


Indicates whether the text is formula if it starts with "=".

**Returns:**
boolean
### hasTextQualifier() {#hasTextQualifier--}
```
public boolean hasTextQualifier()
```


Whether there is text qualifier for cell value. Default is true.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isMultiEncoded() {#isMultiEncoded--}
```
public boolean isMultiEncoded()
```


True means that the file contains several encoding.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAutoFilter(boolean value) {#setAutoFilter-boolean-}
```
public void setAutoFilter(boolean value)
```


For the description of this property, please see [getAutoFilter()](../../com.aspose.cells/loadoptions\#getAutoFilter--)

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

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


For the description of this property, please see [getConvertNumericData()](../../com.aspose.cells/abstracttextloadoptions\#getConvertNumericData--)

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

### setExtendToNextSheet(boolean value) {#setExtendToNextSheet-boolean-}
```
public void setExtendToNextSheet(boolean value)
```


For the description of this property, please see [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFontConfigs(IndividualFontConfigs value) {#setFontConfigs-com.aspose.cells.IndividualFontConfigs-}
```
public void setFontConfigs(IndividualFontConfigs value)
```


For the description of this property, please see [getFontConfigs()](../../com.aspose.cells/loadoptions\#getFontConfigs--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs) |  |

### setHasFormula(boolean value) {#setHasFormula-boolean-}
```
public void setHasFormula(boolean value)
```


For the description of this property, please see [hasFormula()](../../com.aspose.cells/txtloadoptions\#hasFormula--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHasTextQualifier(boolean value) {#setHasTextQualifier-boolean-}
```
public void setHasTextQualifier(boolean value)
```


For the description of this property, please see [hasTextQualifier()](../../com.aspose.cells/txtloadoptions\#hasTextQualifier--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

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

### setMultiEncoded(boolean value) {#setMultiEncoded-boolean-}
```
public void setMultiEncoded(boolean value)
```


For the description of this property, please see [isMultiEncoded()](../../com.aspose.cells/txtloadoptions\#isMultiEncoded--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

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

### setPreferredParsers(ICustomParser[] value) {#setPreferredParsers-com.aspose.cells.ICustomParser---}
```
public void setPreferredParsers(ICustomParser[] value)
```


For the description of this property, please see [getPreferredParsers()](../../com.aspose.cells/txtloadoptions\#getPreferredParsers--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ICustomParser\[\]](../../com.aspose.cells/icustomparser) |  |

### setRegion(int value) {#setRegion-int-}
```
public void setRegion(int value)
```


For the description of this property, please see [getRegion()](../../com.aspose.cells/loadoptions\#getRegion--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```


For the description of this property, please see [getSeparator()](../../com.aspose.cells/txtloadoptions\#getSeparator--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | char |  |

### setSeparatorString(String value) {#setSeparatorString-java.lang.String-}
```
public void setSeparatorString(String value)
```


For the description of this property, please see [getSeparatorString()](../../com.aspose.cells/txtloadoptions\#getSeparatorString--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

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

### setTextQualifier(char value) {#setTextQualifier-char-}
```
public void setTextQualifier(char value)
```


For the description of this property, please see [getTextQualifier()](../../com.aspose.cells/txtloadoptions\#getTextQualifier--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | char |  |

### setTreatConsecutiveDelimitersAsOne(boolean value) {#setTreatConsecutiveDelimitersAsOne-boolean-}
```
public void setTreatConsecutiveDelimitersAsOne(boolean value)
```


For the description of this property, please see [getTreatConsecutiveDelimitersAsOne()](../../com.aspose.cells/txtloadoptions\#getTreatConsecutiveDelimitersAsOne--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setTreatQuotePrefixAsValue(boolean value) {#setTreatQuotePrefixAsValue-boolean-}
```
public void setTreatQuotePrefixAsValue(boolean value)
```


For the description of this property, please see [getTreatQuotePrefixAsValue()](../../com.aspose.cells/txtloadoptions\#getTreatQuotePrefixAsValue--)

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

