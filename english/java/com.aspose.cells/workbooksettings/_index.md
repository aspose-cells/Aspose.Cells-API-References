---
title: WorkbookSettings
second_title: Aspose.Cells for Java API Reference
description: Represents all settings of the workbook.
type: docs
url: /java/com.aspose.cells/workbooksettings/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookSettings
```

Represents all settings of the workbook.

**Example**

```
         Workbook workbook = new Workbook();
 
         WorkbookSettings settings = workbook.getSettings();
 
         //do your business
```
## Methods

| Method | Description |
| --- | --- |
| [dispose()](#dispose--) | Releases resources. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | Gets the author of the file. |
| [getAutoCompressPictures()](#getAutoCompressPictures--) | Specifies a boolean value that indicates the application automatically compressed pictures in the workbook. |
| [getAutoRecover()](#getAutoRecover--) | Indicates whether the file is marked for auto-recovery. |
| [getBuildVersion()](#getBuildVersion--) | Specifies the incremental public release of the application. |
| [getCheckCompatibility()](#getCheckCompatibility--) | Indicates whether check compatibility with earlier versions when saving workbook. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | Indicates whether checking custom number format when setting Style.Custom. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Whether check restriction of excel file when user modify cells related objects. |
| [getClass()](#getClass--) |  |
| [getCompliance()](#getCompliance--) | Specifies the OOXML version for the output document. |
| [getCrashSave()](#getCrashSave--) | indicates whether the application last saved the workbook file after a crash. |
| [getDataExtractLoad()](#getDataExtractLoad--) | indicates whether the application last opened the workbook for data recovery. |
| [getDate1904()](#getDate1904--) | Gets a value which represents if the workbook uses the 1904 date system. |
| [getDefaultImageResolution()](#getDefaultImageResolution--) | Gets default resolution of image. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Gets the settings for default values of style-related properties for this workbook. |
| [getDiscardImageEditData()](#getDiscardImageEditData--) | Indicates whether discarding editting image data. |
| [getDisplayDrawingObjects()](#getDisplayDrawingObjects--) | Indicates whether and how to show objects in the workbook. |
| [getEnableMacros()](#getEnableMacros--) | Enable macros; |
| [getFirstVisibleTab()](#getFirstVisibleTab--) | Gets the first visible worksheet tab. |
| [getFormulaSettings()](#getFormulaSettings--) | Gets the settings for formula-related features. |
| [getGlobalizationSettings()](#getGlobalizationSettings--) | Gets the globalization settings. |
| [getHidePivotFieldList()](#getHidePivotFieldList--) | Gets whether hide the field list for the PivotTable. |
| [getLanguageCode()](#getLanguageCode--) | Gets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [getLocale()](#getLocale--) | Gets the Locale used by this workbook. |
| [getMaxColumn()](#getMaxColumn--) | Gets the max column index, zero-based. |
| [getMaxRow()](#getMaxRow--) | Gets the max row index, zero-based. |
| [getMaxRowsOfSharedFormula()](#getMaxRowsOfSharedFormula--) | Gets the max row number of shared formula. |
| [getMaxUniqueItemsPerField()](#getMaxUniqueItemsPerField--) | Gets the limitation of unique items per field |
| [getMemorySetting()](#getMemorySetting--) | Gets the memory usage options. |
| [getNumberDecimalSeparator()](#getNumberDecimalSeparator--) | Gets the decimal separator for formatting/parsing numeric values. |
| [getNumberGroupSeparator()](#getNumberGroupSeparator--) | Gets the character that separates groups of digits to the left of the decimal in numeric values. |
| [getPaperSize()](#getPaperSize--) | Gets the default print paper size. |
| [getPassword()](#getPassword--) | Represents Workbook file encryption password. |
| [getPropertiesFollowChartPoint()](#getPropertiesFollowChartPoint--) | Indicates whether datapoint properties and datalabels in all charts in this workbook follow their reference. |
| [getProtectionType()](#getProtectionType--) | Gets the protection type of the workbook. |
| [getQuotePrefixToStyle()](#getQuotePrefixToStyle--) | Indicates whether setting [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) property when entering the string value(which starts with single quote mark ) to the cell |
| [getRegion()](#getRegion--) | Gets the regional settings for workbook. |
| [getRemovePersonalInformation()](#getRemovePersonalInformation--) | True if personal information can be removed from the specified workbook. |
| [getRepairLoad()](#getRepairLoad--) | Indicates whether the application last opened the workbook in safe or repair mode. |
| [getResourceProvider()](#getResourceProvider--) | Gets the stream provider for external resource, such as loading image data for picture of type "LinkToFile". |
| [getShared()](#getShared--) | Gets a value that indicates whether the Workbook is shared. |
| [getSheetTabBarWidth()](#getSheetTabBarWidth--) | Width of worksheet tab bar (in 1/1000 of window width). |
| [getShowTabs()](#getShowTabs--) | Gets a value whether the Workbook tabs are displayed. |
| [getSignificantDigits()](#getSignificantDigits--) | Gets the number of significant digits. |
| [getSignificantDigitsType()](#getSignificantDigitsType--) | Gets the type of significant digits for outputing numeric values in this workbook. |
| [getSmartTagOptions()](#getSmartTagOptions--) | Gets the options of the smart tag. |
| [getStreamProvider()](#getStreamProvider--) | Gets the stream provider for external resource. |
| [getThemeFont(int type)](#getThemeFont-int-) | Gets the default theme font name. |
| [getUpdateAdjacentCellsBorder()](#getUpdateAdjacentCellsBorder--) | Indicates whether update adjacent cells' border. |
| [getUpdateLinksType()](#getUpdateLinksType--) | Gets how updates external links when the workbook is opened. |
| [getWarningCallback()](#getWarningCallback--) | Gets warning callback. |
| [getWindowHeight()](#getWindowHeight--) | The height of the window, in unit of point. |
| [getWindowHeightCM()](#getWindowHeightCM--) | The height of the window, in unit of centimeter. |
| [getWindowHeightInch()](#getWindowHeightInch--) | The height of the window, in unit of inch. |
| [getWindowLeft()](#getWindowLeft--) | The distance from the left edge of the client area to the left edge of the window, in unit of point. |
| [getWindowLeftCM()](#getWindowLeftCM--) | The distance from the left edge of the client area to the left edge of the window. |
| [getWindowLeftInch()](#getWindowLeftInch--) | The distance from the left edge of the client area to the left edge of the window. |
| [getWindowTop()](#getWindowTop--) | The distance from the top edge of the client area to the top edge of the window, in unit of point. |
| [getWindowTopCM()](#getWindowTopCM--) | The distance from the top edge of the client area to the top edge of the window, in unit of centimeter. |
| [getWindowTopInch()](#getWindowTopInch--) | The distance from the top edge of the client area to the top edge of the window, in unit of inch. |
| [getWindowWidth()](#getWindowWidth--) | The width of the window, in unit of point. |
| [getWindowWidthCM()](#getWindowWidthCM--) | The width of the window, in unit of centimeter. |
| [getWindowWidthInch()](#getWindowWidthInch--) | The width of the window, in unit of inch. |
| [getWpsCompatibility()](#getWpsCompatibility--) | Indicates whether to be compatible with WPS. |
| [getWriteProtection()](#getWriteProtection--) | Provides access to the workbook write protection options. |
| [hashCode()](#hashCode--) |  |
| [isDefaultEncrypted()](#isDefaultEncrypted--) | Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked. |
| [isEncrypted()](#isEncrypted--) | Gets a value that indicates whether a password is required to open this workbook. |
| [isHScrollBarVisible()](#isHScrollBarVisible--) | Gets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar. |
| [isHidden()](#isHidden--) | Indicates whether this workbook is hidden. |
| [isMinimized()](#isMinimized--) | Represents whether the generated spreadsheet will be opened Minimized. |
| [isProtected()](#isProtected--) | Gets a value that indicates whether the structure or window of the Workbook is protected. |
| [isVScrollBarVisible()](#isVScrollBarVisible--) | Gets a value indicating whether the generated spreadsheet will contain a vertical scroll bar. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Sets the author of the file. |
| [setAutoCompressPictures(boolean value)](#setAutoCompressPictures-boolean-) | Specifies a boolean value that indicates the application automatically compressed pictures in the workbook. |
| [setAutoRecover(boolean value)](#setAutoRecover-boolean-) | Indicates whether the file is marked for auto-recovery. |
| [setBuildVersion(String value)](#setBuildVersion-java.lang.String-) | Specifies the incremental public release of the application. |
| [setCheckCompatibility(boolean value)](#setCheckCompatibility-boolean-) | Indicates whether check compatibility with earlier versions when saving workbook. |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | Indicates whether checking custom number format when setting Style.Custom. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Whether check restriction of excel file when user modify cells related objects. |
| [setCompliance(int value)](#setCompliance-int-) | Specifies the OOXML version for the output document. |
| [setCrashSave(boolean value)](#setCrashSave-boolean-) | indicates whether the application last saved the workbook file after a crash. |
| [setDataExtractLoad(boolean value)](#setDataExtractLoad-boolean-) | indicates whether the application last opened the workbook for data recovery. |
| [setDate1904(boolean value)](#setDate1904-boolean-) | Sets a value which represents if the workbook uses the 1904 date system. |
| [setDefaultEncrypted(boolean value)](#setDefaultEncrypted-boolean-) | Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked. |
| [setDefaultImageResolution(int value)](#setDefaultImageResolution-int-) | Sets default resolution of image. |
| [setDiscardImageEditData(boolean value)](#setDiscardImageEditData-boolean-) | Indicates whether discarding editting image data. |
| [setDisplayDrawingObjects(int value)](#setDisplayDrawingObjects-int-) | Indicates whether and how to show objects in the workbook. |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | Enable macros; |
| [setFirstVisibleTab(int value)](#setFirstVisibleTab-int-) | Sets the first visible worksheet tab. |
| [setGlobalizationSettings(GlobalizationSettings value)](#setGlobalizationSettings-com.aspose.cells.GlobalizationSettings-) | Sets the globalization settings. |
| [setHScrollBarVisible(boolean value)](#setHScrollBarVisible-boolean-) | Sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar. |
| [setHidden(boolean value)](#setHidden-boolean-) | Indicates whether this workbook is hidden. |
| [setHidePivotFieldList(boolean value)](#setHidePivotFieldList-boolean-) | Sets whether hide the field list for the PivotTable. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Sets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | Sets the Locale used by this workbook. |
| [setMaxRowsOfSharedFormula(int value)](#setMaxRowsOfSharedFormula-int-) | Sets the max row number of shared formula. |
| [setMaxUniqueItemsPerField(int value)](#setMaxUniqueItemsPerField-int-) | Sets the limitation of unique items per field |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Sets the memory usage options. |
| [setMinimized(boolean value)](#setMinimized-boolean-) | Represents whether the generated spreadsheet will be opened Minimized. |
| [setNumberDecimalSeparator(char value)](#setNumberDecimalSeparator-char-) | Sets the decimal separator for formatting/parsing numeric values. |
| [setNumberGroupSeparator(char value)](#setNumberGroupSeparator-char-) | Sets the character that separates groups of digits to the left of the decimal in numeric values. |
| [setPageOrientationType(int pageOrientationType)](#setPageOrientationType-int-) | Set the type of print orientation for the whole workbook. |
| [setPaperSize(int value)](#setPaperSize-int-) | Sets the default print paper size. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Represents Workbook file encryption password. |
| [setPropertiesFollowChartPoint(boolean value)](#setPropertiesFollowChartPoint-boolean-) | Indicates whether datapoint properties and datalabels in all charts in this workbook follow their reference. |
| [setQuotePrefixToStyle(boolean value)](#setQuotePrefixToStyle-boolean-) | Indicates whether setting [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) property when entering the string value(which starts with single quote mark ) to the cell |
| [setRegion(int value)](#setRegion-int-) | Sets the regional settings for workbook. |
| [setRemovePersonalInformation(boolean value)](#setRemovePersonalInformation-boolean-) | True if personal information can be removed from the specified workbook. |
| [setRepairLoad(boolean value)](#setRepairLoad-boolean-) | Indicates whether the application last opened the workbook in safe or repair mode. |
| [setResourceProvider(IStreamProvider value)](#setResourceProvider-com.aspose.cells.IStreamProvider-) | Sets the stream provider for external resource, such as loading image data for picture of type "LinkToFile". |
| [setShared(boolean value)](#setShared-boolean-) | Sets a value that indicates whether the Workbook is shared. |
| [setSheetTabBarWidth(int value)](#setSheetTabBarWidth-int-) | Width of worksheet tab bar (in 1/1000 of window width). |
| [setShowTabs(boolean value)](#setShowTabs-boolean-) | Sets a value whether the Workbook tabs are displayed. |
| [setSignificantDigits(int value)](#setSignificantDigits-int-) | Sets the number of significant digits. |
| [setSignificantDigitsType(int value)](#setSignificantDigitsType-int-) | Sets the type of significant digits for outputing numeric values in this workbook. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | Sets the stream provider for external resource. |
| [setUpdateAdjacentCellsBorder(boolean value)](#setUpdateAdjacentCellsBorder-boolean-) | Indicates whether update adjacent cells' border. |
| [setUpdateLinksType(int value)](#setUpdateLinksType-int-) | Sets how updates external links when the workbook is opened. |
| [setVScrollBarVisible(boolean value)](#setVScrollBarVisible-boolean-) | Sets a value indicating whether the generated spreadsheet will contain a vertical scroll bar. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Sets warning callback. |
| [setWindowHeight(double value)](#setWindowHeight-double-) | The height of the window, in unit of point. |
| [setWindowHeightCM(double value)](#setWindowHeightCM-double-) | The height of the window, in unit of centimeter. |
| [setWindowHeightInch(double value)](#setWindowHeightInch-double-) | The height of the window, in unit of inch. |
| [setWindowLeft(double value)](#setWindowLeft-double-) | The distance from the left edge of the client area to the left edge of the window, in unit of point. |
| [setWindowLeftCM(double value)](#setWindowLeftCM-double-) | The distance from the left edge of the client area to the left edge of the window. |
| [setWindowLeftInch(double value)](#setWindowLeftInch-double-) | The distance from the left edge of the client area to the left edge of the window. |
| [setWindowTop(double value)](#setWindowTop-double-) | The distance from the top edge of the client area to the top edge of the window, in unit of point. |
| [setWindowTopCM(double value)](#setWindowTopCM-double-) | The distance from the top edge of the client area to the top edge of the window, in unit of centimeter. |
| [setWindowTopInch(double value)](#setWindowTopInch-double-) | The distance from the top edge of the client area to the top edge of the window, in unit of inch. |
| [setWindowWidth(double value)](#setWindowWidth-double-) | The width of the window, in unit of point. |
| [setWindowWidthCM(double value)](#setWindowWidthCM-double-) | The width of the window, in unit of centimeter. |
| [setWindowWidthInch(double value)](#setWindowWidthInch-double-) | The width of the window, in unit of inch. |
| [setWpsCompatibility(boolean value)](#setWpsCompatibility-boolean-) | Indicates whether to be compatible with WPS. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### dispose() {#dispose--}
```
public void dispose()
```


Releases resources.

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
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Gets the author of the file.

**Remarks**

It''s not set, check [BuiltInDocumentPropertyCollection.getAuthor()](../../com.aspose.cells/builtindocumentpropertycollection\#getAuthor--) first, then check the user of Environment.

**Returns:**
java.lang.String
### getAutoCompressPictures() {#getAutoCompressPictures--}
```
public boolean getAutoCompressPictures()
```


Specifies a boolean value that indicates the application automatically compressed pictures in the workbook.

**Returns:**
boolean
### getAutoRecover() {#getAutoRecover--}
```
public boolean getAutoRecover()
```


Indicates whether the file is marked for auto-recovery.

**Returns:**
boolean
### getBuildVersion() {#getBuildVersion--}
```
public String getBuildVersion()
```


Specifies the incremental public release of the application.

**Returns:**
java.lang.String
### getCheckCompatibility() {#getCheckCompatibility--}
```
public boolean getCheckCompatibility()
```


Indicates whether check compatibility with earlier versions when saving workbook.

**Remarks**

The default value is true. Only for Excel97-2003 xls or xlt files.

**Returns:**
boolean
### getCheckCustomNumberFormat() {#getCheckCustomNumberFormat--}
```
public boolean getCheckCustomNumberFormat()
```


Indicates whether checking custom number format when setting Style.Custom.

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
### getCompliance() {#getCompliance--}
```
public int getCompliance()
```


Specifies the OOXML version for the output document. The default value is Ecma376\_2006.

See [OoxmlCompliance](../../com.aspose.cells/ooxmlcompliance).

**Remarks**

Only for .xlsx files.

**Returns:**
int
### getCrashSave() {#getCrashSave--}
```
public boolean getCrashSave()
```


indicates whether the application last saved the workbook file after a crash.

**Returns:**
boolean
### getDataExtractLoad() {#getDataExtractLoad--}
```
public boolean getDataExtractLoad()
```


indicates whether the application last opened the workbook for data recovery.

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


Gets a value which represents if the workbook uses the 1904 date system.

**Returns:**
boolean
### getDefaultImageResolution() {#getDefaultImageResolution--}
```
public int getDefaultImageResolution()
```


Gets default resolution of image.

**Returns:**
int
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```
public DefaultStyleSettings getDefaultStyleSettings()
```


Gets the settings for default values of style-related properties for this workbook.

**Returns:**
[DefaultStyleSettings](../../com.aspose.cells/defaultstylesettings)
### getDiscardImageEditData() {#getDiscardImageEditData--}
```
public boolean getDiscardImageEditData()
```


Indicates whether discarding editting image data.

**Returns:**
boolean
### getDisplayDrawingObjects() {#getDisplayDrawingObjects--}
```
public int getDisplayDrawingObjects()
```


Indicates whether and how to show objects in the workbook.

See [DisplayDrawingObjects](../../com.aspose.cells/displaydrawingobjects).

**Returns:**
int
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


Enable macros;

**Remarks**

Now it only works when copying a worksheet to other worksheet in a workbook.

**Returns:**
boolean
### getFirstVisibleTab() {#getFirstVisibleTab--}
```
public int getFirstVisibleTab()
```


Gets the first visible worksheet tab.

**Returns:**
int
### getFormulaSettings() {#getFormulaSettings--}
```
public FormulaSettings getFormulaSettings()
```


Gets the settings for formula-related features.

**Returns:**
[FormulaSettings](../../com.aspose.cells/formulasettings)
### getGlobalizationSettings() {#getGlobalizationSettings--}
```
public GlobalizationSettings getGlobalizationSettings()
```


Gets the globalization settings.

**Returns:**
[GlobalizationSettings](../../com.aspose.cells/globalizationsettings)
### getHidePivotFieldList() {#getHidePivotFieldList--}
```
public boolean getHidePivotFieldList()
```


Gets whether hide the field list for the PivotTable.

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
### getLocale() {#getLocale--}
```
public Locale getLocale()
```


Gets the Locale used by this workbook.

**Remarks**

Returns null if neither Locale nor [getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) is set.

**Returns:**
java.util.Locale
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Gets the max column index, zero-based.

**Remarks**

Returns 255 if the file format is Excel97-2003;

**Returns:**
int
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Gets the max row index, zero-based.

**Remarks**

Returns 65535 if the file format is Excel97-2003;

**Returns:**
int
### getMaxRowsOfSharedFormula() {#getMaxRowsOfSharedFormula--}
```
public int getMaxRowsOfSharedFormula()
```


Gets the max row number of shared formula.

**Remarks**

If the number is too large, the autofilter works very slow in MS Excel 2013.

**Returns:**
int
### getMaxUniqueItemsPerField() {#getMaxUniqueItemsPerField--}
```
public int getMaxUniqueItemsPerField()
```


Gets the limitation of unique items per field

**Remarks**

**Returns:**
int
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


Gets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets.

See [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

For more details about memory mode, please see [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Returns:**
int
### getNumberDecimalSeparator() {#getNumberDecimalSeparator--}
```
public char getNumberDecimalSeparator()
```


Gets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Region.

**Returns:**
char
### getNumberGroupSeparator() {#getNumberGroupSeparator--}
```
public char getNumberGroupSeparator()
```


Gets the character that separates groups of digits to the left of the decimal in numeric values. Default is the group separator of current Region.

**Returns:**
char
### getPaperSize() {#getPaperSize--}
```
public int getPaperSize()
```


Gets the default print paper size.

See [PaperSizeType](../../com.aspose.cells/papersizetype).

**Remarks**

If there is no setting about paper size,MS Excel will use default printer's setting.

**Returns:**
int
### getPassword() {#getPassword--}
```
public String getPassword()
```


Represents Workbook file encryption password.

**Returns:**
java.lang.String
### getPropertiesFollowChartPoint() {#getPropertiesFollowChartPoint--}
```
public boolean getPropertiesFollowChartPoint()
```


Indicates whether datapoint properties and datalabels in all charts in this workbook follow their reference.

**Returns:**
boolean
### getProtectionType() {#getProtectionType--}
```
public int getProtectionType()
```


Gets the protection type of the workbook.

See [ProtectionType](../../com.aspose.cells/protectiontype).

**Returns:**
int
### getQuotePrefixToStyle() {#getQuotePrefixToStyle--}
```
public boolean getQuotePrefixToStyle()
```


Indicates whether setting [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) property when entering the string value(which starts with single quote mark ) to the cell

**Returns:**
boolean
### getRegion() {#getRegion--}
```
public int getRegion()
```


Gets the regional settings for workbook.

See [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

1. Regional settings used by Aspose.Cells component for a workbook loaded from template file: i). For an XLS file, there are fields defined for regional settings and MS Excel does save regional settings data into the file when saving the XLS file. So, we use the saved region in the template file for the workbook. If you do not want to use the region saved in the XLS file, please reset it to the expected one (such as, CountryCode.Default) after loading the template file. And, we save the user specified value (by this method) into the file too when saving an XLS file. ii). For other file formats, such as, XLSX, XLSB...etc., there is no field defined for regional settings in the file format specification. So, we use the regional settings of application's environment for the workbook. And, the user specified value (by this method) cannot be kept for the generated files with those file formats. 2. For the view effect in MS Excel: The applied regional settings here can take effect only at runtime with Aspose.Cells component and not when viewing the generated file with MS Excel. Even for the generated XLS file in which the specified regional settings data has been saved, when viewing/editing it with MS Excel, the used region to perform formatting by MS Excel is always the default regional settings of the environment where MS Excel is running, not the one saved in the file. It is MS Excel's behavior and cannot be changed by code.

**Returns:**
int
### getRemovePersonalInformation() {#getRemovePersonalInformation--}
```
public boolean getRemovePersonalInformation()
```


True if personal information can be removed from the specified workbook.

**Remarks**

**Returns:**
boolean
### getRepairLoad() {#getRepairLoad--}
```
public boolean getRepairLoad()
```


Indicates whether the application last opened the workbook in safe or repair mode.

**Returns:**
boolean
### getResourceProvider() {#getResourceProvider--}
```
public IStreamProvider getResourceProvider()
```


Gets the stream provider for external resource, such as loading image data for picture of type "LinkToFile".

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getShared() {#getShared--}
```
public boolean getShared()
```


Gets a value that indicates whether the Workbook is shared.

**Remarks**

The default value is false.

**Returns:**
boolean
### getSheetTabBarWidth() {#getSheetTabBarWidth--}
```
public int getSheetTabBarWidth()
```


Width of worksheet tab bar (in 1/1000 of window width).

**Returns:**
int
### getShowTabs() {#getShowTabs--}
```
public boolean getShowTabs()
```


Gets a value whether the Workbook tabs are displayed.

**Remarks**

The default value is true.

**Example**

The following code hides the Sheet Tabs and Tab Scrolling Buttons for the spreadsheet.

```
         // Hide the spreadsheet tabs.
         workbook.getSettings().setShowTabs(false);
```

**Returns:**
boolean
### getSignificantDigits() {#getSignificantDigits--}
```
public int getSignificantDigits()
```


Gets the number of significant digits. The default value is [CellsHelper.getSignificantDigits()](../../com.aspose.cells/cellshelper\#getSignificantDigits--).

**Remarks**

Only could be 15 or 17 now. NOTE: This member is now obsolete. Instead, please use [getSignificantDigitsType()](../../com.aspose.cells/workbooksettings\#getSignificantDigitsType--). This property will be removed 12 months later since June 2025. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getSignificantDigitsType() {#getSignificantDigitsType--}
```
public int getSignificantDigitsType()
```


Gets the type of significant digits for outputing numeric values in this workbook. Default value is [CellsHelper.getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--).

See [getSignificantDigitsType()](../../com.aspose.cells/workbooksettings\#getSignificantDigitsType--).

**Returns:**
int
### getSmartTagOptions() {#getSmartTagOptions--}
```
public SmartTagOptions getSmartTagOptions()
```


Gets the options of the smart tag.

**Returns:**
[SmartTagOptions](../../com.aspose.cells/smarttagoptions)
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


Gets the stream provider for external resource.

**Remarks**

NOTE: This member is now obsolete. Instead, please use ResourceProvider property. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getThemeFont(int type) {#getThemeFont-int-}
```
public String getThemeFont(int type)
```


Gets the default theme font name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [FontSchemeType](../../com.aspose.cells/fontschemetype). The scheme type of the font. |

**Returns:**
java.lang.String - 
### getUpdateAdjacentCellsBorder() {#getUpdateAdjacentCellsBorder--}
```
public boolean getUpdateAdjacentCellsBorder()
```


Indicates whether update adjacent cells' border.

**Remarks**

The default value is false. For example: the bottom border of the cell A1 is update, the top border of the cell A2 should be changed too.

**Returns:**
boolean
### getUpdateLinksType() {#getUpdateLinksType--}
```
public int getUpdateLinksType()
```


Gets how updates external links when the workbook is opened.

See [UpdateLinksType](../../com.aspose.cells/updatelinkstype).

**Returns:**
int
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Gets warning callback.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### getWindowHeight() {#getWindowHeight--}
```
public double getWindowHeight()
```


The height of the window, in unit of point.

**Returns:**
double
### getWindowHeightCM() {#getWindowHeightCM--}
```
public double getWindowHeightCM()
```


The height of the window, in unit of centimeter.

**Returns:**
double
### getWindowHeightInch() {#getWindowHeightInch--}
```
public double getWindowHeightInch()
```


The height of the window, in unit of inch.

**Returns:**
double
### getWindowLeft() {#getWindowLeft--}
```
public double getWindowLeft()
```


The distance from the left edge of the client area to the left edge of the window, in unit of point.

**Returns:**
double
### getWindowLeftCM() {#getWindowLeftCM--}
```
public double getWindowLeftCM()
```


The distance from the left edge of the client area to the left edge of the window. In unit of centimeter.

**Returns:**
double
### getWindowLeftInch() {#getWindowLeftInch--}
```
public double getWindowLeftInch()
```


The distance from the left edge of the client area to the left edge of the window. In unit of inch.

**Returns:**
double
### getWindowTop() {#getWindowTop--}
```
public double getWindowTop()
```


The distance from the top edge of the client area to the top edge of the window, in unit of point.

**Returns:**
double
### getWindowTopCM() {#getWindowTopCM--}
```
public double getWindowTopCM()
```


The distance from the top edge of the client area to the top edge of the window, in unit of centimeter.

**Returns:**
double
### getWindowTopInch() {#getWindowTopInch--}
```
public double getWindowTopInch()
```


The distance from the top edge of the client area to the top edge of the window, in unit of inch.

**Returns:**
double
### getWindowWidth() {#getWindowWidth--}
```
public double getWindowWidth()
```


The width of the window, in unit of point.

**Returns:**
double
### getWindowWidthCM() {#getWindowWidthCM--}
```
public double getWindowWidthCM()
```


The width of the window, in unit of centimeter.

**Returns:**
double
### getWindowWidthInch() {#getWindowWidthInch--}
```
public double getWindowWidthInch()
```


The width of the window, in unit of inch.

**Returns:**
double
### getWpsCompatibility() {#getWpsCompatibility--}
```
public boolean getWpsCompatibility()
```


Indicates whether to be compatible with WPS.

**Returns:**
boolean
### getWriteProtection() {#getWriteProtection--}
```
public WriteProtection getWriteProtection()
```


Provides access to the workbook write protection options.

**Returns:**
[WriteProtection](../../com.aspose.cells/writeprotection)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isDefaultEncrypted() {#isDefaultEncrypted--}
```
public boolean isDefaultEncrypted()
```


Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked.

**Remarks**

The default value is false now. It's same as MS Excel 2013.

**Returns:**
boolean
### isEncrypted() {#isEncrypted--}
```
public boolean isEncrypted()
```


Gets a value that indicates whether a password is required to open this workbook.

**Returns:**
boolean
### isHScrollBarVisible() {#isHScrollBarVisible--}
```
public boolean isHScrollBarVisible()
```


Gets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar.

**Remarks**

The default value is true.

**Example**

The following code makes the horizontal scroll bar invisible for the spreadsheet.

```
         // Hide the horizontal scroll bar of the Excel file.
         settings.setHScrollBarVisible(false);
```

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Indicates whether this workbook is hidden.

**Returns:**
boolean
### isMinimized() {#isMinimized--}
```
public boolean isMinimized()
```


Represents whether the generated spreadsheet will be opened Minimized.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Gets a value that indicates whether the structure or window of the Workbook is protected.

**Returns:**
boolean
### isVScrollBarVisible() {#isVScrollBarVisible--}
```
public boolean isVScrollBarVisible()
```


Gets a value indicating whether the generated spreadsheet will contain a vertical scroll bar.

**Remarks**

The default value is true.

**Example**

The following code makes the vertical scroll bar invisible for the spreadsheet.

```
         	// Hide the vertical scroll bar of the Excel file.
         settings.setVScrollBarVisible(false);
```

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




### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Sets the author of the file.

**Remarks**

It''s not set, check [BuiltInDocumentPropertyCollection.getAuthor()](../../com.aspose.cells/builtindocumentpropertycollection\#getAuthor--) first, then check the user of Environment.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setAutoCompressPictures(boolean value) {#setAutoCompressPictures-boolean-}
```
public void setAutoCompressPictures(boolean value)
```


Specifies a boolean value that indicates the application automatically compressed pictures in the workbook.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutoRecover(boolean value) {#setAutoRecover-boolean-}
```
public void setAutoRecover(boolean value)
```


Indicates whether the file is marked for auto-recovery.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setBuildVersion(String value) {#setBuildVersion-java.lang.String-}
```
public void setBuildVersion(String value)
```


Specifies the incremental public release of the application.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setCheckCompatibility(boolean value) {#setCheckCompatibility-boolean-}
```
public void setCheckCompatibility(boolean value)
```


Indicates whether check compatibility with earlier versions when saving workbook.

**Remarks**

The default value is true. Only for Excel97-2003 xls or xlt files.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCheckCustomNumberFormat(boolean value) {#setCheckCustomNumberFormat-boolean-}
```
public void setCheckCustomNumberFormat(boolean value)
```


Indicates whether checking custom number format when setting Style.Custom.

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

### setCompliance(int value) {#setCompliance-int-}
```
public void setCompliance(int value)
```


Specifies the OOXML version for the output document. The default value is Ecma376\_2006.

See [OoxmlCompliance](../../com.aspose.cells/ooxmlcompliance).

**Remarks**

Only for .xlsx files.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCrashSave(boolean value) {#setCrashSave-boolean-}
```
public void setCrashSave(boolean value)
```


indicates whether the application last saved the workbook file after a crash.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDataExtractLoad(boolean value) {#setDataExtractLoad-boolean-}
```
public void setDataExtractLoad(boolean value)
```


indicates whether the application last opened the workbook for data recovery.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


Sets a value which represents if the workbook uses the 1904 date system.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDefaultEncrypted(boolean value) {#setDefaultEncrypted-boolean-}
```
public void setDefaultEncrypted(boolean value)
```


Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked.

**Remarks**

The default value is false now. It's same as MS Excel 2013.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDefaultImageResolution(int value) {#setDefaultImageResolution-int-}
```
public void setDefaultImageResolution(int value)
```


Sets default resolution of image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setDiscardImageEditData(boolean value) {#setDiscardImageEditData-boolean-}
```
public void setDiscardImageEditData(boolean value)
```


Indicates whether discarding editting image data.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDisplayDrawingObjects(int value) {#setDisplayDrawingObjects-int-}
```
public void setDisplayDrawingObjects(int value)
```


Indicates whether and how to show objects in the workbook.

See [DisplayDrawingObjects](../../com.aspose.cells/displaydrawingobjects).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


Enable macros;

**Remarks**

Now it only works when copying a worksheet to other worksheet in a workbook.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFirstVisibleTab(int value) {#setFirstVisibleTab-int-}
```
public void setFirstVisibleTab(int value)
```


Sets the first visible worksheet tab.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setGlobalizationSettings(GlobalizationSettings value) {#setGlobalizationSettings-com.aspose.cells.GlobalizationSettings-}
```
public void setGlobalizationSettings(GlobalizationSettings value)
```


Sets the globalization settings.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GlobalizationSettings](../../com.aspose.cells/globalizationsettings) |  |

### setHScrollBarVisible(boolean value) {#setHScrollBarVisible-boolean-}
```
public void setHScrollBarVisible(boolean value)
```


Sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar.

**Remarks**

The default value is true.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Indicates whether this workbook is hidden.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHidePivotFieldList(boolean value) {#setHidePivotFieldList-boolean-}
```
public void setHidePivotFieldList(boolean value)
```


Sets whether hide the field list for the PivotTable.

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

### setLocale(Locale value) {#setLocale-java.util.Locale-}
```
public void setLocale(Locale value)
```


Sets the Locale used by this workbook.

**Remarks**

Returns null if neither Locale nor [getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) is set.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Locale |  |

### setMaxRowsOfSharedFormula(int value) {#setMaxRowsOfSharedFormula-int-}
```
public void setMaxRowsOfSharedFormula(int value)
```


Sets the max row number of shared formula.

**Remarks**

If the number is too large, the autofilter works very slow in MS Excel 2013.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMaxUniqueItemsPerField(int value) {#setMaxUniqueItemsPerField-int-}
```
public void setMaxUniqueItemsPerField(int value)
```


Sets the limitation of unique items per field

**Remarks**

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


Sets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets.

See [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

For more details about memory mode, please see [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMinimized(boolean value) {#setMinimized-boolean-}
```
public void setMinimized(boolean value)
```


Represents whether the generated spreadsheet will be opened Minimized.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setNumberDecimalSeparator(char value) {#setNumberDecimalSeparator-char-}
```
public void setNumberDecimalSeparator(char value)
```


Sets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Region.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | char |  |

### setNumberGroupSeparator(char value) {#setNumberGroupSeparator-char-}
```
public void setNumberGroupSeparator(char value)
```


Sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the group separator of current Region.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | char |  |

### setPageOrientationType(int pageOrientationType) {#setPageOrientationType-int-}
```
public void setPageOrientationType(int pageOrientationType)
```


Set the type of print orientation for the whole workbook.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageOrientationType | int | [PageOrientationType](../../com.aspose.cells/pageorientationtype). The page orientation type |

### setPaperSize(int value) {#setPaperSize-int-}
```
public void setPaperSize(int value)
```


Sets the default print paper size.

See [PaperSizeType](../../com.aspose.cells/papersizetype).

**Remarks**

If there is no setting about paper size,MS Excel will use default printer's setting.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Represents Workbook file encryption password.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setPropertiesFollowChartPoint(boolean value) {#setPropertiesFollowChartPoint-boolean-}
```
public void setPropertiesFollowChartPoint(boolean value)
```


Indicates whether datapoint properties and datalabels in all charts in this workbook follow their reference.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setQuotePrefixToStyle(boolean value) {#setQuotePrefixToStyle-boolean-}
```
public void setQuotePrefixToStyle(boolean value)
```


Indicates whether setting [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) property when entering the string value(which starts with single quote mark ) to the cell

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setRegion(int value) {#setRegion-int-}
```
public void setRegion(int value)
```


Sets the regional settings for workbook.

See [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

1. Regional settings used by Aspose.Cells component for a workbook loaded from template file: i). For an XLS file, there are fields defined for regional settings and MS Excel does save regional settings data into the file when saving the XLS file. So, we use the saved region in the template file for the workbook. If you do not want to use the region saved in the XLS file, please reset it to the expected one (such as, CountryCode.Default) after loading the template file. And, we save the user specified value (by this method) into the file too when saving an XLS file. ii). For other file formats, such as, XLSX, XLSB...etc., there is no field defined for regional settings in the file format specification. So, we use the regional settings of application's environment for the workbook. And, the user specified value (by this method) cannot be kept for the generated files with those file formats. 2. For the view effect in MS Excel: The applied regional settings here can take effect only at runtime with Aspose.Cells component and not when viewing the generated file with MS Excel. Even for the generated XLS file in which the specified regional settings data has been saved, when viewing/editing it with MS Excel, the used region to perform formatting by MS Excel is always the default regional settings of the environment where MS Excel is running, not the one saved in the file. It is MS Excel's behavior and cannot be changed by code.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setRemovePersonalInformation(boolean value) {#setRemovePersonalInformation-boolean-}
```
public void setRemovePersonalInformation(boolean value)
```


True if personal information can be removed from the specified workbook.

**Remarks**

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setRepairLoad(boolean value) {#setRepairLoad-boolean-}
```
public void setRepairLoad(boolean value)
```


Indicates whether the application last opened the workbook in safe or repair mode.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setResourceProvider(IStreamProvider value) {#setResourceProvider-com.aspose.cells.IStreamProvider-}
```
public void setResourceProvider(IStreamProvider value)
```


Sets the stream provider for external resource, such as loading image data for picture of type "LinkToFile".

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setShared(boolean value) {#setShared-boolean-}
```
public void setShared(boolean value)
```


Sets a value that indicates whether the Workbook is shared.

**Remarks**

The default value is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSheetTabBarWidth(int value) {#setSheetTabBarWidth-int-}
```
public void setSheetTabBarWidth(int value)
```


Width of worksheet tab bar (in 1/1000 of window width).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setShowTabs(boolean value) {#setShowTabs-boolean-}
```
public void setShowTabs(boolean value)
```


Sets a value whether the Workbook tabs are displayed.

**Remarks**

The default value is true.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSignificantDigits(int value) {#setSignificantDigits-int-}
```
public void setSignificantDigits(int value)
```


Sets the number of significant digits. The default value is [CellsHelper.getSignificantDigits()](../../com.aspose.cells/cellshelper\#getSignificantDigits--).

**Remarks**

Only could be 15 or 17 now. NOTE: This member is now obsolete. Instead, please use [getSignificantDigitsType()](../../com.aspose.cells/workbooksettings\#getSignificantDigitsType--). This property will be removed 12 months later since June 2025. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setSignificantDigitsType(int value) {#setSignificantDigitsType-int-}
```
public void setSignificantDigitsType(int value)
```


Sets the type of significant digits for outputing numeric values in this workbook. Default value is [CellsHelper.getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--).

See [getSignificantDigitsType()](../../com.aspose.cells/workbooksettings\#getSignificantDigitsType--).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


Sets the stream provider for external resource.

**Remarks**

NOTE: This member is now obsolete. Instead, please use ResourceProvider property. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setUpdateAdjacentCellsBorder(boolean value) {#setUpdateAdjacentCellsBorder-boolean-}
```
public void setUpdateAdjacentCellsBorder(boolean value)
```


Indicates whether update adjacent cells' border.

**Remarks**

The default value is false. For example: the bottom border of the cell A1 is update, the top border of the cell A2 should be changed too.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setUpdateLinksType(int value) {#setUpdateLinksType-int-}
```
public void setUpdateLinksType(int value)
```


Sets how updates external links when the workbook is opened.

See [UpdateLinksType](../../com.aspose.cells/updatelinkstype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setVScrollBarVisible(boolean value) {#setVScrollBarVisible-boolean-}
```
public void setVScrollBarVisible(boolean value)
```


Sets a value indicating whether the generated spreadsheet will contain a vertical scroll bar.

**Remarks**

The default value is true.

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

### setWindowHeight(double value) {#setWindowHeight-double-}
```
public void setWindowHeight(double value)
```


The height of the window, in unit of point.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWindowHeightCM(double value) {#setWindowHeightCM-double-}
```
public void setWindowHeightCM(double value)
```


The height of the window, in unit of centimeter.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWindowHeightInch(double value) {#setWindowHeightInch-double-}
```
public void setWindowHeightInch(double value)
```


The height of the window, in unit of inch.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWindowLeft(double value) {#setWindowLeft-double-}
```
public void setWindowLeft(double value)
```


The distance from the left edge of the client area to the left edge of the window, in unit of point.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWindowLeftCM(double value) {#setWindowLeftCM-double-}
```
public void setWindowLeftCM(double value)
```


The distance from the left edge of the client area to the left edge of the window. In unit of centimeter.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWindowLeftInch(double value) {#setWindowLeftInch-double-}
```
public void setWindowLeftInch(double value)
```


The distance from the left edge of the client area to the left edge of the window. In unit of inch.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWindowTop(double value) {#setWindowTop-double-}
```
public void setWindowTop(double value)
```


The distance from the top edge of the client area to the top edge of the window, in unit of point.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWindowTopCM(double value) {#setWindowTopCM-double-}
```
public void setWindowTopCM(double value)
```


The distance from the top edge of the client area to the top edge of the window, in unit of centimeter.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWindowTopInch(double value) {#setWindowTopInch-double-}
```
public void setWindowTopInch(double value)
```


The distance from the top edge of the client area to the top edge of the window, in unit of inch.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWindowWidth(double value) {#setWindowWidth-double-}
```
public void setWindowWidth(double value)
```


The width of the window, in unit of point.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWindowWidthCM(double value) {#setWindowWidthCM-double-}
```
public void setWindowWidthCM(double value)
```


The width of the window, in unit of centimeter.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWindowWidthInch(double value) {#setWindowWidthInch-double-}
```
public void setWindowWidthInch(double value)
```


The width of the window, in unit of inch.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWpsCompatibility(boolean value) {#setWpsCompatibility-boolean-}
```
public void setWpsCompatibility(boolean value)
```


Indicates whether to be compatible with WPS.

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

