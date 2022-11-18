---
title: XmlLoadOptions
second_title: Aspose.Cells for Java API Reference
description: Represents the options of loading xml.
type: docs
weight: 668
url: /java/com.aspose.cells/xmlloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LoadOptions](../../com.aspose.cells/loadoptions)
```
public class XmlLoadOptions extends LoadOptions
```

Represents the options of loading xml.
## Constructors

| Constructor | Description |
| --- | --- |
| [XmlLoadOptions()](#XmlLoadOptions--) | Represents the options of loading xml file. |
| [XmlLoadOptions(int type)](#XmlLoadOptions-int-) | Represents the options of loading xml file. |
## Methods

| Method | Description |
| --- | --- |
| [containsMultipleWorksheets()](#containsMultipleWorksheets--) | Indicates whether importing xml as multiple worksheets. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Indicates whether auto filtering the data when loading the files. |
| [getAutoFitterOptions()](#getAutoFitterOptions--) | Gets and sets the auto fitter options Only for xlsx ,spreadsheetML file now. |
| [getCheckDataValid()](#getCheckDataValid--) | Check whether data is valid in the template file. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Whether check restriction of excel file when user modify cells related objects. |
| [getClass()](#getClass--) |  |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Gets the default style settings for initializing styles of the workbook |
| [getFontConfigs()](#getFontConfigs--) | Gets and sets individual font configs. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Ignore the data which are not printed if directly printing the file Only for xlsx file. |
| [getInterruptMonitor()](#getInterruptMonitor--) | Gets and sets the interrupt monitor. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. |
| [getLanguageCode()](#getLanguageCode--) | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [getLightCellsDataHandler()](#getLightCellsDataHandler--) | The data handler for processing cells data when reading template file. |
| [getLoadFilter()](#getLoadFilter--) | The filter to denote how to load data. |
| [getLoadFormat()](#getLoadFormat--) | Gets the load format. |
| [getLocale()](#getLocale--) | Gets and sets the Locale used for workbook at the time the file was loaded. |
| [getMemorySetting()](#getMemorySetting--) | Gets or sets the memory usage options. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Indicates whether parsing the formula when reading the file. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Indicates whether parsing pivot cached records when loading the file. |
| [getPassword()](#getPassword--) | Gets and set the password of the workbook. |
| [getRegion()](#getRegion--) | Gets or sets the system regional settings based on CountryCode at the time the file was loaded. |
| [getStandardFont()](#getStandardFont--) | Sets the default standard font name NOTE: This member is now obsolete. |
| [getStandardFontSize()](#getStandardFontSize--) | Sets the default standard font size. |
| [getStartCell()](#getStartCell--) | Gets and sets the start cell. |
| [getWarningCallback()](#getWarningCallback--) | Gets or sets warning callback. |
| [hashCode()](#hashCode--) |  |
| [isXmlMap()](#isXmlMap--) | Indicates whether mapping xml to Excel. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | For the description of this property, please see \#getAutoFilter().getAutoFilter() |
| [setAutoFitterOptions(AutoFitterOptions value)](#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-) | For the description of this property, please see \#getAutoFitterOptions().getAutoFitterOptions() |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | For the description of this property, please see \#getCheckDataValid().getCheckDataValid() |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | For the description of this property, please see \#getCheckExcelRestriction().getCheckExcelRestriction() |
| [setContainsMultipleWorksheets(boolean value)](#setContainsMultipleWorksheets-boolean-) | For the description of this property, please see \#containsMultipleWorksheets().containsMultipleWorksheets() |
| [setFontConfigs(IndividualFontConfigs value)](#setFontConfigs-com.aspose.cells.IndividualFontConfigs-) | For the description of this property, please see \#getFontConfigs().getFontConfigs() |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | For the description of this property, please see \#getIgnoreNotPrinted().getIgnoreNotPrinted() |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | For the description of this property, please see \#getInterruptMonitor().getInterruptMonitor() |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | For the description of this property, please see \#getKeepUnparsedData().getKeepUnparsedData() |
| [setLanguageCode(int value)](#setLanguageCode-int-) | For the description of this property, please see \#getLanguageCode().getLanguageCode() |
| [setLightCellsDataHandler(LightCellsDataHandler value)](#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-) | For the description of this property, please see \#getLightCellsDataHandler().getLightCellsDataHandler() |
| [setLoadFilter(LoadFilter value)](#setLoadFilter-com.aspose.cells.LoadFilter-) | For the description of this property, please see \#getLoadFilter().getLoadFilter() |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | For the description of this property, please see \#getLocale().getLocale() |
| [setMemorySetting(int value)](#setMemorySetting-int-) | For the description of this property, please see \#getMemorySetting().getMemorySetting() |
| [setPaperSize(int type)](#setPaperSize-int-) | Sets the default print paper size from default printer's setting. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | For the description of this property, please see \#getParsingFormulaOnOpen().getParsingFormulaOnOpen() |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | For the description of this property, please see \#getParsingPivotCachedRecords().getParsingPivotCachedRecords() |
| [setPassword(String value)](#setPassword-java.lang.String-) | For the description of this property, please see \#getPassword().getPassword() |
| [setRegion(int value)](#setRegion-int-) | For the description of this property, please see \#getRegion().getRegion() |
| [setStandardFont(String value)](#setStandardFont-java.lang.String-) | For the description of this property, please see \#getStandardFont().getStandardFont() |
| [setStandardFontSize(double value)](#setStandardFontSize-double-) | For the description of this property, please see \#getStandardFontSize().getStandardFontSize() |
| [setStartCell(String value)](#setStartCell-java.lang.String-) | For the description of this property, please see \#getStartCell().getStartCell() |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) |  |
| [setXmlMap(boolean value)](#setXmlMap-boolean-) | For the description of this property, please see \#isXmlMap().isXmlMap() |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### XmlLoadOptions() {#XmlLoadOptions--}
```
public XmlLoadOptions()
```


Represents the options of loading xml file.

### XmlLoadOptions(int type) {#XmlLoadOptions-int-}
```
public XmlLoadOptions(int type)
```


Represents the options of loading xml file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | The load format type. |

### containsMultipleWorksheets() {#containsMultipleWorksheets--}
```
public boolean containsMultipleWorksheets()
```


Indicates whether importing xml as multiple worksheets.

**Returns:**
boolean
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
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```
public DefaultStyleSettings getDefaultStyleSettings()
```


Gets the default style settings for initializing styles of the workbook

**Returns:**
[DefaultStyleSettings](../../com.aspose.cells/defaultstylesettings)
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
### getStartCell() {#getStartCell--}
```
public String getStartCell()
```


Gets and sets the start cell. Only works when the file is not speadsheetML or mapping xml to Excel.

**Returns:**
java.lang.String
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
### isXmlMap() {#isXmlMap--}
```
public boolean isXmlMap()
```


Indicates whether mapping xml to Excel. The default value is false.

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


For the description of this property, please see \#getAutoFilter().getAutoFilter()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutoFitterOptions(AutoFitterOptions value) {#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-}
```
public void setAutoFitterOptions(AutoFitterOptions value)
```


For the description of this property, please see \#getAutoFitterOptions().getAutoFitterOptions()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) |  |

### setCheckDataValid(boolean value) {#setCheckDataValid-boolean-}
```
public void setCheckDataValid(boolean value)
```


For the description of this property, please see \#getCheckDataValid().getCheckDataValid()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


For the description of this property, please see \#getCheckExcelRestriction().getCheckExcelRestriction()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setContainsMultipleWorksheets(boolean value) {#setContainsMultipleWorksheets-boolean-}
```
public void setContainsMultipleWorksheets(boolean value)
```


For the description of this property, please see \#containsMultipleWorksheets().containsMultipleWorksheets()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFontConfigs(IndividualFontConfigs value) {#setFontConfigs-com.aspose.cells.IndividualFontConfigs-}
```
public void setFontConfigs(IndividualFontConfigs value)
```


For the description of this property, please see \#getFontConfigs().getFontConfigs()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs) |  |

### setIgnoreNotPrinted(boolean value) {#setIgnoreNotPrinted-boolean-}
```
public void setIgnoreNotPrinted(boolean value)
```


For the description of this property, please see \#getIgnoreNotPrinted().getIgnoreNotPrinted()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setInterruptMonitor(AbstractInterruptMonitor value) {#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-}
```
public void setInterruptMonitor(AbstractInterruptMonitor value)
```


For the description of this property, please see \#getInterruptMonitor().getInterruptMonitor()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) |  |

### setKeepUnparsedData(boolean value) {#setKeepUnparsedData-boolean-}
```
public void setKeepUnparsedData(boolean value)
```


For the description of this property, please see \#getKeepUnparsedData().getKeepUnparsedData()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


For the description of this property, please see \#getLanguageCode().getLanguageCode()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLightCellsDataHandler(LightCellsDataHandler value) {#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-}
```
public void setLightCellsDataHandler(LightCellsDataHandler value)
```


For the description of this property, please see \#getLightCellsDataHandler().getLightCellsDataHandler()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LightCellsDataHandler](../../com.aspose.cells/lightcellsdatahandler) |  |

### setLoadFilter(LoadFilter value) {#setLoadFilter-com.aspose.cells.LoadFilter-}
```
public void setLoadFilter(LoadFilter value)
```


For the description of this property, please see \#getLoadFilter().getLoadFilter()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LoadFilter](../../com.aspose.cells/loadfilter) |  |

### setLocale(Locale value) {#setLocale-java.util.Locale-}
```
public void setLocale(Locale value)
```


For the description of this property, please see \#getLocale().getLocale()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Locale |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


For the description of this property, please see \#getMemorySetting().getMemorySetting()

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


For the description of this property, please see \#getParsingFormulaOnOpen().getParsingFormulaOnOpen()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setParsingPivotCachedRecords(boolean value) {#setParsingPivotCachedRecords-boolean-}
```
public void setParsingPivotCachedRecords(boolean value)
```


For the description of this property, please see \#getParsingPivotCachedRecords().getParsingPivotCachedRecords()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


For the description of this property, please see \#getPassword().getPassword()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setRegion(int value) {#setRegion-int-}
```
public void setRegion(int value)
```


For the description of this property, please see \#getRegion().getRegion()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setStandardFont(String value) {#setStandardFont-java.lang.String-}
```
public void setStandardFont(String value)
```


For the description of this property, please see \#getStandardFont().getStandardFont()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setStandardFontSize(double value) {#setStandardFontSize-double-}
```
public void setStandardFontSize(double value)
```


For the description of this property, please see \#getStandardFontSize().getStandardFontSize()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setStartCell(String value) {#setStartCell-java.lang.String-}
```
public void setStartCell(String value)
```


For the description of this property, please see \#getStartCell().getStartCell()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

### setXmlMap(boolean value) {#setXmlMap-boolean-}
```
public void setXmlMap(boolean value)
```


For the description of this property, please see \#isXmlMap().isXmlMap()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

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

