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
| [getAutoFitterOptions()](#getAutoFitterOptions--) | Gets the auto fitter options |
| [getCheckDataValid()](#getCheckDataValid--) | Check whether data is valid in the template file. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Whether check restriction of excel file when user modify cells related objects. |
| [getClass()](#getClass--) |  |
| [getConvertDateTimeData()](#getConvertDateTimeData--) | Gets a value that indicates whether the string in text file is converted to date data. |
| [getConvertNumericData()](#getConvertNumericData--) | Gets a value that indicates whether the string in text file is converted to numeric data. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Gets the default style settings for initializing styles of the workbook |
| [getEncoding()](#getEncoding--) | Gets the default encoding. |
| [getExtendToNextSheet()](#getExtendToNextSheet--) | Whether extends data to next sheet when the rows or columns of data exceed limit. |
| [getFontConfigs()](#getFontConfigs--) | Gets individual font configs. |
| [getHeaderColumnsCount()](#getHeaderColumnsCount--) | The count of header columns to be repeated for extended sheets. |
| [getHeaderRowsCount()](#getHeaderRowsCount--) | The count of header rows to be repeated for extended sheets. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Ignore the data which are not printed if directly printing the file |
| [getIgnoreUselessShapes()](#getIgnoreUselessShapes--) | Indicates whether ignoring useless shapes. |
| [getInterruptMonitor()](#getInterruptMonitor--) | Gets the interrupt monitor. |
| [getKeepPrecision()](#getKeepPrecision--) | Indicates whether not parsing a string value if the length is 15. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. |
| [getLanguageCode()](#getLanguageCode--) | Gets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [getLightCellsDataHandler()](#getLightCellsDataHandler--) | The data handler for processing cells data when reading template file. |
| [getLoadFilter()](#getLoadFilter--) | The filter to denote how to load data. |
| [getLoadFormat()](#getLoadFormat--) | Gets the load format. |
| [getLoadStyleStrategy()](#getLoadStyleStrategy--) | Indicates the strategy to apply style for parsed values when converting string value to number or datetime. |
| [getLocale()](#getLocale--) | Gets the regional settings used for the Workbook that will be loaded. |
| [getMaxColumnCount()](#getMaxColumnCount--) | The maximum count of columns to be imported for one sheet. |
| [getMaxRowCount()](#getMaxRowCount--) | The maximum count of rows to be imported for one sheet. |
| [getMemorySetting()](#getMemorySetting--) | Gets the memory mode for loaded workbook. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Indicates whether parsing the formula when reading the file. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Indicates whether parsing pivot cached records when loading the file. |
| [getPassword()](#getPassword--) | Gets the password of the workbook. |
| [getPreferredParsers()](#getPreferredParsers--) | Gets preferred value parsers for loading text file. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. |
| [getRegion()](#getRegion--) | Gets the regional settings used for the Workbook that will be loaded. |
| [getSeparator()](#getSeparator--) | Gets character separator of text file. |
| [getSeparatorString()](#getSeparatorString--) | Gets a string value as separator. |
| [getStandardFont()](#getStandardFont--) | Sets the default standard font name |
| [getStandardFontSize()](#getStandardFontSize--) | Sets the default standard font size. |
| [getTextQualifier()](#getTextQualifier--) | Specifies the text qualifier for cell values. |
| [getTreatConsecutiveDelimitersAsOne()](#getTreatConsecutiveDelimitersAsOne--) | Whether consecutive delimiters should be treated as one. |
| [getTreatQuotePrefixAsValue()](#getTreatQuotePrefixAsValue--) | Indicates whether the leading single quote sign should be taken as part of the value of one cell. |
| [getWarningCallback()](#getWarningCallback--) | Gets warning callback. |
| [hasFormula()](#hasFormula--) | Indicates whether the text is formula if it starts with "=". |
| [hasTextQualifier()](#hasTextQualifier--) | Whether there is text qualifier for cell value. |
| [hashCode()](#hashCode--) |  |
| [isMultiEncoded()](#isMultiEncoded--) | True means that the file contains several encoding. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Indicates whether auto filtering the data when loading the files. |
| [setAutoFitterOptions(AutoFitterOptions value)](#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-) | Sets the auto fitter options |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Check whether data is valid in the template file. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Whether check restriction of excel file when user modify cells related objects. |
| [setConvertDateTimeData(boolean value)](#setConvertDateTimeData-boolean-) | Sets a value that indicates whether the string in text file is converted to date data. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Sets a value that indicates whether the string in text file is converted to numeric data. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Sets the default encoding. |
| [setExtendToNextSheet(boolean value)](#setExtendToNextSheet-boolean-) | Whether extends data to next sheet when the rows or columns of data exceed limit. |
| [setFontConfigs(IndividualFontConfigs value)](#setFontConfigs-com.aspose.cells.IndividualFontConfigs-) | Sets individual font configs. |
| [setHasFormula(boolean value)](#setHasFormula-boolean-) | Indicates whether the text is formula if it starts with "=". |
| [setHasTextQualifier(boolean value)](#setHasTextQualifier-boolean-) | Whether there is text qualifier for cell value. |
| [setHeaderColumnsCount(int value)](#setHeaderColumnsCount-int-) | The count of header columns to be repeated for extended sheets. |
| [setHeaderRowsCount(int value)](#setHeaderRowsCount-int-) | The count of header rows to be repeated for extended sheets. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Ignore the data which are not printed if directly printing the file |
| [setIgnoreUselessShapes(boolean value)](#setIgnoreUselessShapes-boolean-) | Indicates whether ignoring useless shapes. |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | Sets the interrupt monitor. |
| [setKeepPrecision(boolean value)](#setKeepPrecision-boolean-) | Indicates whether not parsing a string value if the length is 15. |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Sets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [setLightCellsDataHandler(LightCellsDataHandler value)](#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-) | The data handler for processing cells data when reading template file. |
| [setLoadFilter(LoadFilter value)](#setLoadFilter-com.aspose.cells.LoadFilter-) | The filter to denote how to load data. |
| [setLoadStyleStrategy(int value)](#setLoadStyleStrategy-int-) | Indicates the strategy to apply style for parsed values when converting string value to number or datetime. |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | Sets the regional settings used for the Workbook that will be loaded. |
| [setMaxColumnCount(int value)](#setMaxColumnCount-int-) | The maximum count of columns to be imported for one sheet. |
| [setMaxRowCount(int value)](#setMaxRowCount-int-) | The maximum count of rows to be imported for one sheet. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Sets the memory mode for loaded workbook. |
| [setMultiEncoded(boolean value)](#setMultiEncoded-boolean-) | True means that the file contains several encoding. |
| [setPaperSize(int type)](#setPaperSize-int-) | Sets the default print paper size from default printer's setting. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Indicates whether parsing the formula when reading the file. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Indicates whether parsing pivot cached records when loading the file. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Sets the password of the workbook. |
| [setPreferredParsers(ICustomParser[] value)](#setPreferredParsers-com.aspose.cells.ICustomParser---) | Sets preferred value parsers for loading text file. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. |
| [setRegion(int value)](#setRegion-int-) | Sets the regional settings used for the Workbook that will be loaded. |
| [setSeparator(char value)](#setSeparator-char-) | Sets character separator of text file. |
| [setSeparatorString(String value)](#setSeparatorString-java.lang.String-) | Sets a string value as separator. |
| [setStandardFont(String value)](#setStandardFont-java.lang.String-) | Sets the default standard font name |
| [setStandardFontSize(double value)](#setStandardFontSize-double-) | Sets the default standard font size. |
| [setTextQualifier(char value)](#setTextQualifier-char-) | Specifies the text qualifier for cell values. |
| [setTreatConsecutiveDelimitersAsOne(boolean value)](#setTreatConsecutiveDelimitersAsOne-boolean-) | Whether consecutive delimiters should be treated as one. |
| [setTreatQuotePrefixAsValue(boolean value)](#setTreatQuotePrefixAsValue-boolean-) | Indicates whether the leading single quote sign should be taken as part of the value of one cell. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Sets warning callback. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### TxtLoadOptions() {#TxtLoadOptions--}
```
public TxtLoadOptions()
```


Creates the options for loading text file.

**Remarks**

The default load file type is CSV .

### TxtLoadOptions(int loadFormat) {#TxtLoadOptions-int-}
```
public TxtLoadOptions(int loadFormat)
```


Creates the options for loading text file.

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
### getAutoFilter() {#getAutoFilter--}
```
public boolean getAutoFilter()
```


Indicates whether auto filtering the data when loading the files.

**Remarks**

Sometimes although autofilter is set, the corresponding rows is not hidden in the file. Now only works for SpreadSheetML file.

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
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Gets the default encoding. Only applies for csv file.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getExtendToNextSheet() {#getExtendToNextSheet--}
```
public boolean getExtendToNextSheet()
```


Whether extends data to next sheet when the rows or columns of data exceed limit. Default is false.

**Remarks**

If this property is true, extra data will be put into next sheet behind current one (if current sheet is the last one, new sheet will be appended to current workbook). If this property is false, the data exceeding limit will be ignored.

**Returns:**
boolean
### getFontConfigs() {#getFontConfigs--}
```
public IndividualFontConfigs getFontConfigs()
```


Gets individual font configs. Only works for the [Workbook](../../com.aspose.cells/workbook) which uses this [LoadOptions](../../com.aspose.cells/loadoptions) to load.

**Returns:**
[IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs)
### getHeaderColumnsCount() {#getHeaderColumnsCount--}
```
public int getHeaderColumnsCount()
```


The count of header columns to be repeated for extended sheets.

**Remarks**

The header columns specified by this property will be duplicated for those extended sheets. This property only takes effect when [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--) is true.

**Returns:**
int
### getHeaderRowsCount() {#getHeaderRowsCount--}
```
public int getHeaderRowsCount()
```


The count of header rows to be repeated for extended sheets.

**Remarks**

The header rows specified by this property will be duplicated for those extended sheets. This property only takes effect when [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--) is true.

**Returns:**
int
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
### getMaxColumnCount() {#getMaxColumnCount--}
```
public int getMaxColumnCount()
```


The maximum count of columns to be imported for one sheet.

**Remarks**

Those columns exceeding this limit will be ignored or extended to next sheet according to [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--). This count includes the header columns([getHeaderColumnsCount()](../../com.aspose.cells/txtloadoptions\#getHeaderColumnsCount--)). The maximum value of it is the column limit of corresponding file format, such as for xlsx file it 16384. If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.

**Returns:**
int
### getMaxRowCount() {#getMaxRowCount--}
```
public int getMaxRowCount()
```


The maximum count of rows to be imported for one sheet.

**Remarks**

Those rows exceeding this limit will be ignored or extended to next sheet according to [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--). This count includes the header rows([getHeaderRowsCount()](../../com.aspose.cells/txtloadoptions\#getHeaderRowsCount--)). The maximum allowed value of it is the row limit of corresponding file format, such as for xlsx file it 1048576. If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.

**Returns:**
int
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
### getPreferredParsers() {#getPreferredParsers--}
```
public ICustomParser[] getPreferredParsers()
```


Gets preferred value parsers for loading text file.

**Remarks**

parsers[0] is the parser will be used for the first column in text template file, parsers[1] is the parser will be used for the second column, ...etc. The last one(parsers[parsers.length-1]) will be used for all other columns start from parsers.length-1. If one item is null, the corresponding column will be parsed by the default parser of Aspose.Cells.

**Returns:**
com.aspose.cells.ICustomParser[]
### getPreservePaddingSpacesInFormula() {#getPreservePaddingSpacesInFormula--}
```
public boolean getPreservePaddingSpacesInFormula()
```


Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false.

**Remarks**

After loading workbook from template file with this option, [FormulaSettings.getPreservePaddingSpaces()](../../com.aspose.cells/formulasettings\#getPreservePaddingSpaces--) will be set to the same value with this property.

**Returns:**
boolean
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
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```


Gets character separator of text file.

**Returns:**
char
### getSeparatorString() {#getSeparatorString--}
```
public String getSeparatorString()
```


Gets a string value as separator.

**Returns:**
java.lang.String
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
### getTextQualifier() {#getTextQualifier--}
```
public char getTextQualifier()
```


Specifies the text qualifier for cell values. Default qualifier is '"'.

**Remarks**

When setting this property, [hasTextQualifier()](../../com.aspose.cells/txtloadoptions\#hasTextQualifier--) will become true automatically.

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


Indicates whether auto filtering the data when loading the files.

**Remarks**

Sometimes although autofilter is set, the corresponding rows is not hidden in the file. Now only works for SpreadSheetML file.

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

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Sets a value that indicates whether the string in text file is converted to numeric data. Default value is true.

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

### setExtendToNextSheet(boolean value) {#setExtendToNextSheet-boolean-}
```
public void setExtendToNextSheet(boolean value)
```


Whether extends data to next sheet when the rows or columns of data exceed limit. Default is false.

**Remarks**

If this property is true, extra data will be put into next sheet behind current one (if current sheet is the last one, new sheet will be appended to current workbook). If this property is false, the data exceeding limit will be ignored.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

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

### setHasTextQualifier(boolean value) {#setHasTextQualifier-boolean-}
```
public void setHasTextQualifier(boolean value)
```


Whether there is text qualifier for cell value. Default is true.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHeaderColumnsCount(int value) {#setHeaderColumnsCount-int-}
```
public void setHeaderColumnsCount(int value)
```


The count of header columns to be repeated for extended sheets.

**Remarks**

The header columns specified by this property will be duplicated for those extended sheets. This property only takes effect when [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--) is true.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setHeaderRowsCount(int value) {#setHeaderRowsCount-int-}
```
public void setHeaderRowsCount(int value)
```


The count of header rows to be repeated for extended sheets.

**Remarks**

The header rows specified by this property will be duplicated for those extended sheets. This property only takes effect when [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--) is true.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

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

### setMaxColumnCount(int value) {#setMaxColumnCount-int-}
```
public void setMaxColumnCount(int value)
```


The maximum count of columns to be imported for one sheet.

**Remarks**

Those columns exceeding this limit will be ignored or extended to next sheet according to [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--). This count includes the header columns([getHeaderColumnsCount()](../../com.aspose.cells/txtloadoptions\#getHeaderColumnsCount--)). The maximum value of it is the column limit of corresponding file format, such as for xlsx file it 16384. If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMaxRowCount(int value) {#setMaxRowCount-int-}
```
public void setMaxRowCount(int value)
```


The maximum count of rows to be imported for one sheet.

**Remarks**

Those rows exceeding this limit will be ignored or extended to next sheet according to [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--). This count includes the header rows([getHeaderRowsCount()](../../com.aspose.cells/txtloadoptions\#getHeaderRowsCount--)). The maximum allowed value of it is the row limit of corresponding file format, such as for xlsx file it 1048576. If this property has not been specified or the specified value is not positive, then the maximum limit will be used too.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

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

### setMultiEncoded(boolean value) {#setMultiEncoded-boolean-}
```
public void setMultiEncoded(boolean value)
```


True means that the file contains several encoding.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

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

### setPreferredParsers(ICustomParser[] value) {#setPreferredParsers-com.aspose.cells.ICustomParser---}
```
public void setPreferredParsers(ICustomParser[] value)
```


Sets preferred value parsers for loading text file.

**Remarks**

parsers[0] is the parser will be used for the first column in text template file, parsers[1] is the parser will be used for the second column, ...etc. The last one(parsers[parsers.length-1]) will be used for all other columns start from parsers.length-1. If one item is null, the corresponding column will be parsed by the default parser of Aspose.Cells.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ICustomParser\[\]](../../com.aspose.cells/icustomparser) |  |

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

### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```


Sets character separator of text file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | char |  |

### setSeparatorString(String value) {#setSeparatorString-java.lang.String-}
```
public void setSeparatorString(String value)
```


Sets a string value as separator.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

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

### setTextQualifier(char value) {#setTextQualifier-char-}
```
public void setTextQualifier(char value)
```


Specifies the text qualifier for cell values. Default qualifier is '"'.

**Remarks**

When setting this property, [hasTextQualifier()](../../com.aspose.cells/txtloadoptions\#hasTextQualifier--) will become true automatically.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | char |  |

### setTreatConsecutiveDelimitersAsOne(boolean value) {#setTreatConsecutiveDelimitersAsOne-boolean-}
```
public void setTreatConsecutiveDelimitersAsOne(boolean value)
```


Whether consecutive delimiters should be treated as one.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setTreatQuotePrefixAsValue(boolean value) {#setTreatQuotePrefixAsValue-boolean-}
```
public void setTreatQuotePrefixAsValue(boolean value)
```


Indicates whether the leading single quote sign should be taken as part of the value of one cell. Default is true. If it is false, the leading single quote will be removed from corresponding cell's value and [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) will be set as true for the cell.

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

