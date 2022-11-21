---
title: WorkbookSettings
second_title: Aspose.Cells for Java API Reference
description: Represents all settings of the workbook.
type: docs
weight: 659
url: /java/com.aspose.cells/workbooksettings/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookSettings
```

Represents all settings of the workbook.

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
| [getAuthor()](#getAuthor--) | the author of the file. |
| [getAutoCompressPictures()](#getAutoCompressPictures--) | Specifies a boolean value that indicates the application automatically compressed pictures in the workbook. |
| [getAutoRecover()](#getAutoRecover--) | Indicates whether the file is mark for auto-recovery. |
| [getBuildVersion()](#getBuildVersion--) | Specifies the incremental public release of the application. |
| [getCalcMode()](#getCalcMode--) | It specifies whether to calculate formulas manually, automatically or automatically except for multiple table operations. |
| [getCalcStackSize()](#getCalcStackSize--) | Specifies the stack size for calculating cells recursively. |
| [getCalculationId()](#getCalculationId--) | Specifies the version of the calculation engine used to calculate values in the workbook. |
| [getCheckCompatibility()](#getCheckCompatibility--) | Indicates whether check compatibility with earlier versions when saving workbook. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | Indicates whether checking custom number format when setting Style.Custom. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Whether check restriction of excel file when user modify cells related objects. |
| [getClass()](#getClass--) |  |
| [getCompliance()](#getCompliance--) | Specifies the OOXML version for the output document. |
| [getCrashSave()](#getCrashSave--) | indicates whether the application last saved the workbook file after a crash. |
| [getCreateCalcChain()](#getCreateCalcChain--) | Whether creates calculated formulas chain. |
| [getDataExtractLoad()](#getDataExtractLoad--) | indicates whether the application last opened the workbook for data recovery. |
| [getDate1904()](#getDate1904--) | a value which represents if the workbook uses the 1904 date system. |
| [getDisplayDrawingObjects()](#getDisplayDrawingObjects--) | Indicates whether and how to show objects in the workbook. |
| [getEnableMacros()](#getEnableMacros--) | Enable macros; Now it only works when copying a worksheet to other worksheet in a workbook. |
| [getFirstVisibleTab()](#getFirstVisibleTab--) | the first visible worksheet tab. |
| [getForceFullCalculate()](#getForceFullCalculate--) | Fully calculates every time when a calculation is triggered. |
| [getFormulaSettings()](#getFormulaSettings--) | Gets the settings for formula-related features. |
| [getGlobalizationSettings()](#getGlobalizationSettings--) | the globalization settings. |
| [getHidePivotFieldList()](#getHidePivotFieldList--) | whether hide the field list for the PivotTable. |
| [getIteration()](#getIteration--) | Indicates whether enable iterative calculation to resolve circular references. |
| [getLanguageCode()](#getLanguageCode--) | the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [getLocale()](#getLocale--) | the Locale used by this workbook. |
| [getMaxChange()](#getMaxChange--) | Returns or sets the maximum number of change to resolve a circular reference. |
| [getMaxColumn()](#getMaxColumn--) | Gets the max column index, zero-based. |
| [getMaxIteration()](#getMaxIteration--) | Returns or sets the maximum number of iterations to resolve a circular reference. |
| [getMaxRow()](#getMaxRow--) | Gets the max row index, zero-based. |
| [getMaxRowsOfSharedFormula()](#getMaxRowsOfSharedFormula--) | the max row number of shared formula. |
| [getMemorySetting()](#getMemorySetting--) | the memory usage options. |
| [getNumberDecimalSeparator()](#getNumberDecimalSeparator--) | the decimal separator for formatting/parsing numeric values. |
| [getNumberGroupSeparator()](#getNumberGroupSeparator--) | the character that separates groups of digits to the left of the decimal in numeric values. |
| [getPaperSize()](#getPaperSize--) | the default print paper size. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Indicates whether parsing the formula when reading the file. |
| [getPassword()](#getPassword--) | Represents Workbook file encryption password. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | True if calculations in this workbook will be done using only the precision of the numbers as they're displayed NOTE: This member is now obsolete. |
| [getProtectionType()](#getProtectionType--) | Gets the protection type of the workbook. |
| [getQuotePrefixToStyle()](#getQuotePrefixToStyle--) | Indicates whether setting [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) property when entering the string value(which starts with single quote mark ) to the cell |
| [getReCalculateOnOpen()](#getReCalculateOnOpen--) | Indicates whether re-calculate all formulas on opening file. |
| [getRecalculateBeforeSave()](#getRecalculateBeforeSave--) | Indicates whether to recalculate before saving the document. |
| [getRegion()](#getRegion--) | the regional settings for workbook. 1. |
| [getRemovePersonalInformation()](#getRemovePersonalInformation--) | True if personal information can be removed from the specified workbook. |
| [getRepairLoad()](#getRepairLoad--) | Indicates whether the application last opened the workbook in safe or repair mode. |
| [getResourceProvider()](#getResourceProvider--) | the stream provider for external resource, such as loading image data for picture of type "LinkToFile". |
| [getShared()](#getShared--) | a value that indicates whether the Workbook is shared. |
| [getSheetTabBarWidth()](#getSheetTabBarWidth--) | Width of worksheet tab bar (in 1/1000 of window width). |
| [getShowTabs()](#getShowTabs--) | a value whether the Workbook tabs are displayed. |
| [getSignificantDigits()](#getSignificantDigits--) | the number of significant digits. |
| [getStreamProvider()](#getStreamProvider--) | the stream provider for external resource. |
| [getThemeFont(int type)](#getThemeFont-int-) | Gets the default theme font name. |
| [getUpdateAdjacentCellsBorder()](#getUpdateAdjacentCellsBorder--) | Indicates whether update adjacent cells' border. |
| [getUpdateLinksType()](#getUpdateLinksType--) | how updates external links when the workbook is opened. |
| [getWarningCallback()](#getWarningCallback--) | warning callback. |
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
| [getWriteProtection()](#getWriteProtection--) | Provides access to the workbook write protection options. |
| [hashCode()](#hashCode--) |  |
| [isDefaultEncrypted()](#isDefaultEncrypted--) | Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked. |
| [isEncrypted()](#isEncrypted--) | Gets a value that indicates whether a password is required to open this workbook. |
| [isHScrollBarVisible()](#isHScrollBarVisible--) | a value indicating whether the generated spreadsheet will contain a horizontal scroll bar. |
| [isHidden()](#isHidden--) | Indicates whether this workbook is hidden. |
| [isMinimized()](#isMinimized--) | Represents whether the generated spreadsheet will be opened Minimized. |
| [isProtected()](#isProtected--) | Gets a value that indicates whether the structure or window of the Workbook is protected. |
| [isVScrollBarVisible()](#isVScrollBarVisible--) | a value indicating whether the generated spreadsheet will contain a vertical scroll bar. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | For the description of this property, please see [getAuthor()](../../com.aspose.cells/workbooksettings\#getAuthor--) |
| [setAutoCompressPictures(boolean value)](#setAutoCompressPictures-boolean-) | For the description of this property, please see [getAutoCompressPictures()](../../com.aspose.cells/workbooksettings\#getAutoCompressPictures--) |
| [setAutoRecover(boolean value)](#setAutoRecover-boolean-) | For the description of this property, please see [getAutoRecover()](../../com.aspose.cells/workbooksettings\#getAutoRecover--) |
| [setBuildVersion(String value)](#setBuildVersion-java.lang.String-) | For the description of this property, please see [getBuildVersion()](../../com.aspose.cells/workbooksettings\#getBuildVersion--) |
| [setCalcMode(int value)](#setCalcMode-int-) | For the description of this property, please see [getCalcMode()](../../com.aspose.cells/workbooksettings\#getCalcMode--) |
| [setCalcStackSize(int value)](#setCalcStackSize-int-) | For the description of this property, please see [getCalcStackSize()](../../com.aspose.cells/workbooksettings\#getCalcStackSize--) |
| [setCalculationId(String value)](#setCalculationId-java.lang.String-) | For the description of this property, please see [getCalculationId()](../../com.aspose.cells/workbooksettings\#getCalculationId--) |
| [setCheckCompatibility(boolean value)](#setCheckCompatibility-boolean-) | For the description of this property, please see [getCheckCompatibility()](../../com.aspose.cells/workbooksettings\#getCheckCompatibility--) |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | For the description of this property, please see [getCheckCustomNumberFormat()](../../com.aspose.cells/workbooksettings\#getCheckCustomNumberFormat--) |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | For the description of this property, please see [getCheckExcelRestriction()](../../com.aspose.cells/workbooksettings\#getCheckExcelRestriction--) |
| [setCompliance(int value)](#setCompliance-int-) | For the description of this property, please see [getCompliance()](../../com.aspose.cells/workbooksettings\#getCompliance--) |
| [setCrashSave(boolean value)](#setCrashSave-boolean-) | For the description of this property, please see [getCrashSave()](../../com.aspose.cells/workbooksettings\#getCrashSave--) |
| [setCreateCalcChain(boolean value)](#setCreateCalcChain-boolean-) | For the description of this property, please see [getCreateCalcChain()](../../com.aspose.cells/workbooksettings\#getCreateCalcChain--) |
| [setDataExtractLoad(boolean value)](#setDataExtractLoad-boolean-) | For the description of this property, please see [getDataExtractLoad()](../../com.aspose.cells/workbooksettings\#getDataExtractLoad--) |
| [setDate1904(boolean value)](#setDate1904-boolean-) | For the description of this property, please see [getDate1904()](../../com.aspose.cells/workbooksettings\#getDate1904--) |
| [setDefaultEncrypted(boolean value)](#setDefaultEncrypted-boolean-) | For the description of this property, please see [isDefaultEncrypted()](../../com.aspose.cells/workbooksettings\#isDefaultEncrypted--) |
| [setDisplayDrawingObjects(int value)](#setDisplayDrawingObjects-int-) | For the description of this property, please see [getDisplayDrawingObjects()](../../com.aspose.cells/workbooksettings\#getDisplayDrawingObjects--) |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | For the description of this property, please see [getEnableMacros()](../../com.aspose.cells/workbooksettings\#getEnableMacros--) |
| [setFirstVisibleTab(int value)](#setFirstVisibleTab-int-) | For the description of this property, please see [getFirstVisibleTab()](../../com.aspose.cells/workbooksettings\#getFirstVisibleTab--) |
| [setForceFullCalculate(boolean value)](#setForceFullCalculate-boolean-) | For the description of this property, please see [getForceFullCalculate()](../../com.aspose.cells/workbooksettings\#getForceFullCalculate--) |
| [setGlobalizationSettings(GlobalizationSettings value)](#setGlobalizationSettings-com.aspose.cells.GlobalizationSettings-) | For the description of this property, please see [getGlobalizationSettings()](../../com.aspose.cells/workbooksettings\#getGlobalizationSettings--) |
| [setHScrollBarVisible(boolean value)](#setHScrollBarVisible-boolean-) | For the description of this property, please see [isHScrollBarVisible()](../../com.aspose.cells/workbooksettings\#isHScrollBarVisible--) |
| [setHidden(boolean value)](#setHidden-boolean-) | For the description of this property, please see [isHidden()](../../com.aspose.cells/workbooksettings\#isHidden--) |
| [setHidePivotFieldList(boolean value)](#setHidePivotFieldList-boolean-) | For the description of this property, please see [getHidePivotFieldList()](../../com.aspose.cells/workbooksettings\#getHidePivotFieldList--) |
| [setIteration(boolean value)](#setIteration-boolean-) | For the description of this property, please see [getIteration()](../../com.aspose.cells/workbooksettings\#getIteration--) |
| [setLanguageCode(int value)](#setLanguageCode-int-) | For the description of this property, please see [getLanguageCode()](../../com.aspose.cells/workbooksettings\#getLanguageCode--) |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | For the description of this property, please see [getLocale()](../../com.aspose.cells/workbooksettings\#getLocale--) |
| [setMaxChange(double value)](#setMaxChange-double-) | For the description of this property, please see [getMaxChange()](../../com.aspose.cells/workbooksettings\#getMaxChange--) |
| [setMaxIteration(int value)](#setMaxIteration-int-) | For the description of this property, please see [getMaxIteration()](../../com.aspose.cells/workbooksettings\#getMaxIteration--) |
| [setMaxRowsOfSharedFormula(int value)](#setMaxRowsOfSharedFormula-int-) | For the description of this property, please see [getMaxRowsOfSharedFormula()](../../com.aspose.cells/workbooksettings\#getMaxRowsOfSharedFormula--) |
| [setMemorySetting(int value)](#setMemorySetting-int-) | For the description of this property, please see [getMemorySetting()](../../com.aspose.cells/workbooksettings\#getMemorySetting--) |
| [setMinimized(boolean value)](#setMinimized-boolean-) | For the description of this property, please see [isMinimized()](../../com.aspose.cells/workbooksettings\#isMinimized--) |
| [setNumberDecimalSeparator(char value)](#setNumberDecimalSeparator-char-) | For the description of this property, please see [getNumberDecimalSeparator()](../../com.aspose.cells/workbooksettings\#getNumberDecimalSeparator--) |
| [setNumberGroupSeparator(char value)](#setNumberGroupSeparator-char-) | For the description of this property, please see [getNumberGroupSeparator()](../../com.aspose.cells/workbooksettings\#getNumberGroupSeparator--) |
| [setPageOrientationType(int pageOrientationType)](#setPageOrientationType-int-) | Set the type of print orientation for the whole workbook. |
| [setPaperSize(int value)](#setPaperSize-int-) | For the description of this property, please see [getPaperSize()](../../com.aspose.cells/workbooksettings\#getPaperSize--) |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | For the description of this property, please see [getParsingFormulaOnOpen()](../../com.aspose.cells/workbooksettings\#getParsingFormulaOnOpen--) |
| [setPassword(String value)](#setPassword-java.lang.String-) | For the description of this property, please see [getPassword()](../../com.aspose.cells/workbooksettings\#getPassword--) |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | For the description of this property, please see [getPrecisionAsDisplayed()](../../com.aspose.cells/workbooksettings\#getPrecisionAsDisplayed--) |
| [setQuotePrefixToStyle(boolean value)](#setQuotePrefixToStyle-boolean-) | For the description of this property, please see [getQuotePrefixToStyle()](../../com.aspose.cells/workbooksettings\#getQuotePrefixToStyle--) |
| [setReCalculateOnOpen(boolean value)](#setReCalculateOnOpen-boolean-) | For the description of this property, please see [getReCalculateOnOpen()](../../com.aspose.cells/workbooksettings\#getReCalculateOnOpen--) |
| [setRecalculateBeforeSave(boolean value)](#setRecalculateBeforeSave-boolean-) | For the description of this property, please see [getRecalculateBeforeSave()](../../com.aspose.cells/workbooksettings\#getRecalculateBeforeSave--) |
| [setRegion(int value)](#setRegion-int-) | For the description of this property, please see [getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) |
| [setRemovePersonalInformation(boolean value)](#setRemovePersonalInformation-boolean-) | For the description of this property, please see [getRemovePersonalInformation()](../../com.aspose.cells/workbooksettings\#getRemovePersonalInformation--) |
| [setRepairLoad(boolean value)](#setRepairLoad-boolean-) | For the description of this property, please see [getRepairLoad()](../../com.aspose.cells/workbooksettings\#getRepairLoad--) |
| [setResourceProvider(IStreamProvider value)](#setResourceProvider-com.aspose.cells.IStreamProvider-) | For the description of this property, please see [getResourceProvider()](../../com.aspose.cells/workbooksettings\#getResourceProvider--) |
| [setShared(boolean value)](#setShared-boolean-) | For the description of this property, please see [getShared()](../../com.aspose.cells/workbooksettings\#getShared--) |
| [setSheetTabBarWidth(int value)](#setSheetTabBarWidth-int-) | For the description of this property, please see [getSheetTabBarWidth()](../../com.aspose.cells/workbooksettings\#getSheetTabBarWidth--) |
| [setShowTabs(boolean value)](#setShowTabs-boolean-) | For the description of this property, please see [getShowTabs()](../../com.aspose.cells/workbooksettings\#getShowTabs--) |
| [setSignificantDigits(int value)](#setSignificantDigits-int-) | For the description of this property, please see [getSignificantDigits()](../../com.aspose.cells/workbooksettings\#getSignificantDigits--) |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | For the description of this property, please see [getStreamProvider()](../../com.aspose.cells/workbooksettings\#getStreamProvider--) |
| [setUpdateAdjacentCellsBorder(boolean value)](#setUpdateAdjacentCellsBorder-boolean-) | For the description of this property, please see [getUpdateAdjacentCellsBorder()](../../com.aspose.cells/workbooksettings\#getUpdateAdjacentCellsBorder--) |
| [setUpdateLinksType(int value)](#setUpdateLinksType-int-) | For the description of this property, please see [getUpdateLinksType()](../../com.aspose.cells/workbooksettings\#getUpdateLinksType--) |
| [setVScrollBarVisible(boolean value)](#setVScrollBarVisible-boolean-) | For the description of this property, please see [isVScrollBarVisible()](../../com.aspose.cells/workbooksettings\#isVScrollBarVisible--) |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) |  |
| [setWindowHeight(double value)](#setWindowHeight-double-) | For the description of this property, please see [getWindowHeight()](../../com.aspose.cells/workbooksettings\#getWindowHeight--) |
| [setWindowHeightCM(double value)](#setWindowHeightCM-double-) | For the description of this property, please see [getWindowHeightCM()](../../com.aspose.cells/workbooksettings\#getWindowHeightCM--) |
| [setWindowHeightInch(double value)](#setWindowHeightInch-double-) | For the description of this property, please see [getWindowHeightInch()](../../com.aspose.cells/workbooksettings\#getWindowHeightInch--) |
| [setWindowLeft(double value)](#setWindowLeft-double-) | For the description of this property, please see [getWindowLeft()](../../com.aspose.cells/workbooksettings\#getWindowLeft--) |
| [setWindowLeftCM(double value)](#setWindowLeftCM-double-) | For the description of this property, please see [getWindowLeftCM()](../../com.aspose.cells/workbooksettings\#getWindowLeftCM--) |
| [setWindowLeftInch(double value)](#setWindowLeftInch-double-) | For the description of this property, please see [getWindowLeftInch()](../../com.aspose.cells/workbooksettings\#getWindowLeftInch--) |
| [setWindowTop(double value)](#setWindowTop-double-) | For the description of this property, please see [getWindowTop()](../../com.aspose.cells/workbooksettings\#getWindowTop--) |
| [setWindowTopCM(double value)](#setWindowTopCM-double-) | For the description of this property, please see [getWindowTopCM()](../../com.aspose.cells/workbooksettings\#getWindowTopCM--) |
| [setWindowTopInch(double value)](#setWindowTopInch-double-) | For the description of this property, please see [getWindowTopInch()](../../com.aspose.cells/workbooksettings\#getWindowTopInch--) |
| [setWindowWidth(double value)](#setWindowWidth-double-) | For the description of this property, please see [getWindowWidth()](../../com.aspose.cells/workbooksettings\#getWindowWidth--) |
| [setWindowWidthCM(double value)](#setWindowWidthCM-double-) | For the description of this property, please see [getWindowWidthCM()](../../com.aspose.cells/workbooksettings\#getWindowWidthCM--) |
| [setWindowWidthInch(double value)](#setWindowWidthInch-double-) | For the description of this property, please see [getWindowWidthInch()](../../com.aspose.cells/workbooksettings\#getWindowWidthInch--) |
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


the author of the file. It''s not set, check [BuiltInDocumentPropertyCollection.getAuthor()](../../com.aspose.cells/builtindocumentpropertycollection\#getAuthor--) first, then check the user of Environment.

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


Indicates whether the file is mark for auto-recovery.

**Returns:**
boolean
### getBuildVersion() {#getBuildVersion--}
```
public String getBuildVersion()
```


Specifies the incremental public release of the application.

**Returns:**
java.lang.String
### getCalcMode() {#getCalcMode--}
```
public int getCalcMode()
```


It specifies whether to calculate formulas manually, automatically or automatically except for multiple table operations. Only sets for MS Excel. Please manually calling Workbook.CalculateFormula() method to calculate formulas with Aspose.Cells. NOTE: This member is now obsolete. Instead, please use FormulaSettings.CalculationMode. This property will be removed 12 months later since February 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getCalcStackSize() {#getCalcStackSize--}
```
public int getCalcStackSize()
```


Specifies the stack size for calculating cells recursively. The large value for this size will give better performance when there are lots of cells need to be calculated recursively. On the other hand, larger value will raise the risk of StackOverflowException. If user gets StackOverflowException when calculating formulas, this value should be decreased. NOTE: This member is now obsolete. Instead, please use CalculationOptions with the specified CalcStackSize when calculating formulas. This property will be removed 12 months later since February 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getCalculationId() {#getCalculationId--}
```
public String getCalculationId()
```


Specifies the version of the calculation engine used to calculate values in the workbook. NOTE: This member is now obsolete. Instead, please use FormulaSettings.CalculationId. This property will be removed 12 months later since February 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
java.lang.String
### getCheckCompatibility() {#getCheckCompatibility--}
```
public boolean getCheckCompatibility()
```


Indicates whether check compatibility with earlier versions when saving workbook. The default value is true. Only for Excel97-2003 xls or xlt files.

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


Specifies the OOXML version for the output document. The default value is Ecma376\_2006. Only for .xlsx files.

**Returns:**
int
### getCrashSave() {#getCrashSave--}
```
public boolean getCrashSave()
```


indicates whether the application last saved the workbook file after a crash.

**Returns:**
boolean
### getCreateCalcChain() {#getCreateCalcChain--}
```
public boolean getCreateCalcChain()
```


Whether creates calculated formulas chain. Default is false. NOTE: This member is now obsolete. Instead, please use FormulaSettings.EnableCalculationChain. This property will be removed 12 months later since February 2022. Aspose apologizes for any inconvenience you may have experienced.

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


a value which represents if the workbook uses the 1904 date system.

**Returns:**
boolean
### getDisplayDrawingObjects() {#getDisplayDrawingObjects--}
```
public int getDisplayDrawingObjects()
```


Indicates whether and how to show objects in the workbook.

**Returns:**
int
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


Enable macros; Now it only works when copying a worksheet to other worksheet in a workbook.

**Returns:**
boolean
### getFirstVisibleTab() {#getFirstVisibleTab--}
```
public int getFirstVisibleTab()
```


the first visible worksheet tab.

**Returns:**
int
### getForceFullCalculate() {#getForceFullCalculate--}
```
public boolean getForceFullCalculate()
```


Fully calculates every time when a calculation is triggered. NOTE: This member is now obsolete. Instead, please use FormulaSettings.ForceFullCalculation. This property will be removed 12 months later since February 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
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


the globalization settings.

**Returns:**
[GlobalizationSettings](../../com.aspose.cells/globalizationsettings)
### getHidePivotFieldList() {#getHidePivotFieldList--}
```
public boolean getHidePivotFieldList()
```


whether hide the field list for the PivotTable.

**Returns:**
boolean
### getIteration() {#getIteration--}
```
public boolean getIteration()
```


Indicates whether enable iterative calculation to resolve circular references. NOTE: This member is now obsolete. Instead, please use FormulaSettings.EnableIterativeCalculation. This property will be removed 12 months later since February 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### getLanguageCode() {#getLanguageCode--}
```
public int getLanguageCode()
```


the user interface language of the Workbook version based on CountryCode that has saved the file.

**Returns:**
int
### getLocale() {#getLocale--}
```
public Locale getLocale()
```


the Locale used by this workbook. Returns null if neither Locale nor [getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) is set.

**Returns:**
java.util.Locale
### getMaxChange() {#getMaxChange--}
```
public double getMaxChange()
```


Returns or sets the maximum number of change to resolve a circular reference. NOTE: This member is now obsolete. Instead, please use FormulaSettings.MaxChange. This property will be removed 12 months later since February 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
double
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Gets the max column index, zero-based. Returns 255 if the file format is Excel97-2003;

**Returns:**
int
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


Returns or sets the maximum number of iterations to resolve a circular reference. NOTE: This member is now obsolete. Instead, please use FormulaSettings.MaxIteration. This property will be removed 12 months later since February 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Gets the max row index, zero-based. Returns 65535 if the file format is Excel97-2003;

**Returns:**
int
### getMaxRowsOfSharedFormula() {#getMaxRowsOfSharedFormula--}
```
public int getMaxRowsOfSharedFormula()
```


the max row number of shared formula. If the number is too large, the autofilter works very slow in MS Excel 2013.

**Returns:**
int
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets.

**Returns:**
int
### getNumberDecimalSeparator() {#getNumberDecimalSeparator--}
```
public char getNumberDecimalSeparator()
```


the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Region.

**Returns:**
char
### getNumberGroupSeparator() {#getNumberGroupSeparator--}
```
public char getNumberGroupSeparator()
```


the character that separates groups of digits to the left of the decimal in numeric values. Default is the group separator of current Region.

**Returns:**
char
### getPaperSize() {#getPaperSize--}
```
public int getPaperSize()
```


the default print paper size. If there is no setting about paper size,MS Excel will use default printer's setting.

**Returns:**
int
### getParsingFormulaOnOpen() {#getParsingFormulaOnOpen--}
```
public boolean getParsingFormulaOnOpen()
```


Indicates whether parsing the formula when reading the file. Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file because the formulas in the files are stored with a string formula. NOTE: This member is now obsolete. Instead, please use LoadOptions.ParsingFormulaOnOpen. This property will be removed 12 months later since January 2020. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### getPassword() {#getPassword--}
```
public String getPassword()
```


Represents Workbook file encryption password.

**Returns:**
java.lang.String
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


True if calculations in this workbook will be done using only the precision of the numbers as they're displayed NOTE: This member is now obsolete. Instead, please use FormulaSettings.PrecisionAsDisplayed. This property will be removed 12 months later since February 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### getProtectionType() {#getProtectionType--}
```
public int getProtectionType()
```


Gets the protection type of the workbook.

**Returns:**
int
### getQuotePrefixToStyle() {#getQuotePrefixToStyle--}
```
public boolean getQuotePrefixToStyle()
```


Indicates whether setting [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) property when entering the string value(which starts with single quote mark ) to the cell

**Returns:**
boolean
### getReCalculateOnOpen() {#getReCalculateOnOpen--}
```
public boolean getReCalculateOnOpen()
```


Indicates whether re-calculate all formulas on opening file. NOTE: This member is now obsolete. Instead, please use FormulaSettings.CalculateOnOpen. This property will be removed 12 months later since February 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### getRecalculateBeforeSave() {#getRecalculateBeforeSave--}
```
public boolean getRecalculateBeforeSave()
```


Indicates whether to recalculate before saving the document. NOTE: This member is now obsolete. Instead, please use FormulaSettings.CalculateOnSave. This property will be removed 12 months later since February 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### getRegion() {#getRegion--}
```
public int getRegion()
```


the regional settings for workbook. 1. Regional settings used by Aspose.Cells component for a workbook loaded from template file: i). For an XLS file, there are fields defined for regional settings and MS Excel does save regional settings data into the file when saving the XLS file. So, we use the saved region in the template file for the workbook. If you do not want to use the region saved in the XLS file, please reset it to the expected one (such as, CountryCode.Default) after loading the template file. And, we save the user specified value (by this method) into the file too when saving an XLS file. ii). For other file formats, such as, XLSX, XLSB...etc., there is no field defined for regional settings in the file format specification. So, we use the regional settings of application's environment for the workbook. And, the user specified value (by this method) cannot be kept for the generated files with those file formats. 2. For the view effect in MS Excel: The applied regional settings here can take effect only at runtime with Aspose.Cells component and not when viewing the generated file with MS Excel. Even for the generated XLS file in which the specified regional settings data has been saved, when viewing/editing it with MS Excel, the used region to perform formatting by MS Excel is always the default regional settings of the environment where MS Excel is running, not the one saved in the file. It is MS Excel's behavior and cannot be changed by code.

**Returns:**
int
### getRemovePersonalInformation() {#getRemovePersonalInformation--}
```
public boolean getRemovePersonalInformation()
```


True if personal information can be removed from the specified workbook.

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


the stream provider for external resource, such as loading image data for picture of type "LinkToFile".

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getShared() {#getShared--}
```
public boolean getShared()
```


a value that indicates whether the Workbook is shared. The default value is false.

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


a value whether the Workbook tabs are displayed. The default value is true.

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


the number of significant digits. The default value is \{@link CellsHelper.getSignificantDigits()\}. Only could be 15 or 17 now.

**Returns:**
int
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


the stream provider for external resource. NOTE: This member is now obsolete. Instead, please use ResourceProvider property. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.

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
| type | int | The scheme type of the font. |

**Returns:**
java.lang.String - 
### getUpdateAdjacentCellsBorder() {#getUpdateAdjacentCellsBorder--}
```
public boolean getUpdateAdjacentCellsBorder()
```


Indicates whether update adjacent cells' border. The default value is false. For example: the bottom border of the cell A1 is update, the top border of the cell A2 should be changed too.

**Returns:**
boolean
### getUpdateLinksType() {#getUpdateLinksType--}
```
public int getUpdateLinksType()
```


how updates external links when the workbook is opened.

**Returns:**
int
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


warning callback.

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


Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked. The default value is false now. It's same as MS Excel 2013.

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


a value indicating whether the generated spreadsheet will contain a horizontal scroll bar. The default value is true.

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


a value indicating whether the generated spreadsheet will contain a vertical scroll bar. The default value is true.

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


For the description of this property, please see [getAuthor()](../../com.aspose.cells/workbooksettings\#getAuthor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setAutoCompressPictures(boolean value) {#setAutoCompressPictures-boolean-}
```
public void setAutoCompressPictures(boolean value)
```


For the description of this property, please see [getAutoCompressPictures()](../../com.aspose.cells/workbooksettings\#getAutoCompressPictures--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutoRecover(boolean value) {#setAutoRecover-boolean-}
```
public void setAutoRecover(boolean value)
```


For the description of this property, please see [getAutoRecover()](../../com.aspose.cells/workbooksettings\#getAutoRecover--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setBuildVersion(String value) {#setBuildVersion-java.lang.String-}
```
public void setBuildVersion(String value)
```


For the description of this property, please see [getBuildVersion()](../../com.aspose.cells/workbooksettings\#getBuildVersion--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setCalcMode(int value) {#setCalcMode-int-}
```
public void setCalcMode(int value)
```


For the description of this property, please see [getCalcMode()](../../com.aspose.cells/workbooksettings\#getCalcMode--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCalcStackSize(int value) {#setCalcStackSize-int-}
```
public void setCalcStackSize(int value)
```


For the description of this property, please see [getCalcStackSize()](../../com.aspose.cells/workbooksettings\#getCalcStackSize--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCalculationId(String value) {#setCalculationId-java.lang.String-}
```
public void setCalculationId(String value)
```


For the description of this property, please see [getCalculationId()](../../com.aspose.cells/workbooksettings\#getCalculationId--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setCheckCompatibility(boolean value) {#setCheckCompatibility-boolean-}
```
public void setCheckCompatibility(boolean value)
```


For the description of this property, please see [getCheckCompatibility()](../../com.aspose.cells/workbooksettings\#getCheckCompatibility--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCheckCustomNumberFormat(boolean value) {#setCheckCustomNumberFormat-boolean-}
```
public void setCheckCustomNumberFormat(boolean value)
```


For the description of this property, please see [getCheckCustomNumberFormat()](../../com.aspose.cells/workbooksettings\#getCheckCustomNumberFormat--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


For the description of this property, please see [getCheckExcelRestriction()](../../com.aspose.cells/workbooksettings\#getCheckExcelRestriction--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCompliance(int value) {#setCompliance-int-}
```
public void setCompliance(int value)
```


For the description of this property, please see [getCompliance()](../../com.aspose.cells/workbooksettings\#getCompliance--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCrashSave(boolean value) {#setCrashSave-boolean-}
```
public void setCrashSave(boolean value)
```


For the description of this property, please see [getCrashSave()](../../com.aspose.cells/workbooksettings\#getCrashSave--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCreateCalcChain(boolean value) {#setCreateCalcChain-boolean-}
```
public void setCreateCalcChain(boolean value)
```


For the description of this property, please see [getCreateCalcChain()](../../com.aspose.cells/workbooksettings\#getCreateCalcChain--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDataExtractLoad(boolean value) {#setDataExtractLoad-boolean-}
```
public void setDataExtractLoad(boolean value)
```


For the description of this property, please see [getDataExtractLoad()](../../com.aspose.cells/workbooksettings\#getDataExtractLoad--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


For the description of this property, please see [getDate1904()](../../com.aspose.cells/workbooksettings\#getDate1904--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDefaultEncrypted(boolean value) {#setDefaultEncrypted-boolean-}
```
public void setDefaultEncrypted(boolean value)
```


For the description of this property, please see [isDefaultEncrypted()](../../com.aspose.cells/workbooksettings\#isDefaultEncrypted--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDisplayDrawingObjects(int value) {#setDisplayDrawingObjects-int-}
```
public void setDisplayDrawingObjects(int value)
```


For the description of this property, please see [getDisplayDrawingObjects()](../../com.aspose.cells/workbooksettings\#getDisplayDrawingObjects--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


For the description of this property, please see [getEnableMacros()](../../com.aspose.cells/workbooksettings\#getEnableMacros--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFirstVisibleTab(int value) {#setFirstVisibleTab-int-}
```
public void setFirstVisibleTab(int value)
```


For the description of this property, please see [getFirstVisibleTab()](../../com.aspose.cells/workbooksettings\#getFirstVisibleTab--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setForceFullCalculate(boolean value) {#setForceFullCalculate-boolean-}
```
public void setForceFullCalculate(boolean value)
```


For the description of this property, please see [getForceFullCalculate()](../../com.aspose.cells/workbooksettings\#getForceFullCalculate--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setGlobalizationSettings(GlobalizationSettings value) {#setGlobalizationSettings-com.aspose.cells.GlobalizationSettings-}
```
public void setGlobalizationSettings(GlobalizationSettings value)
```


For the description of this property, please see [getGlobalizationSettings()](../../com.aspose.cells/workbooksettings\#getGlobalizationSettings--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GlobalizationSettings](../../com.aspose.cells/globalizationsettings) |  |

### setHScrollBarVisible(boolean value) {#setHScrollBarVisible-boolean-}
```
public void setHScrollBarVisible(boolean value)
```


For the description of this property, please see [isHScrollBarVisible()](../../com.aspose.cells/workbooksettings\#isHScrollBarVisible--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


For the description of this property, please see [isHidden()](../../com.aspose.cells/workbooksettings\#isHidden--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHidePivotFieldList(boolean value) {#setHidePivotFieldList-boolean-}
```
public void setHidePivotFieldList(boolean value)
```


For the description of this property, please see [getHidePivotFieldList()](../../com.aspose.cells/workbooksettings\#getHidePivotFieldList--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setIteration(boolean value) {#setIteration-boolean-}
```
public void setIteration(boolean value)
```


For the description of this property, please see [getIteration()](../../com.aspose.cells/workbooksettings\#getIteration--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


For the description of this property, please see [getLanguageCode()](../../com.aspose.cells/workbooksettings\#getLanguageCode--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLocale(Locale value) {#setLocale-java.util.Locale-}
```
public void setLocale(Locale value)
```


For the description of this property, please see [getLocale()](../../com.aspose.cells/workbooksettings\#getLocale--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Locale |  |

### setMaxChange(double value) {#setMaxChange-double-}
```
public void setMaxChange(double value)
```


For the description of this property, please see [getMaxChange()](../../com.aspose.cells/workbooksettings\#getMaxChange--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


For the description of this property, please see [getMaxIteration()](../../com.aspose.cells/workbooksettings\#getMaxIteration--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMaxRowsOfSharedFormula(int value) {#setMaxRowsOfSharedFormula-int-}
```
public void setMaxRowsOfSharedFormula(int value)
```


For the description of this property, please see [getMaxRowsOfSharedFormula()](../../com.aspose.cells/workbooksettings\#getMaxRowsOfSharedFormula--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


For the description of this property, please see [getMemorySetting()](../../com.aspose.cells/workbooksettings\#getMemorySetting--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMinimized(boolean value) {#setMinimized-boolean-}
```
public void setMinimized(boolean value)
```


For the description of this property, please see [isMinimized()](../../com.aspose.cells/workbooksettings\#isMinimized--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setNumberDecimalSeparator(char value) {#setNumberDecimalSeparator-char-}
```
public void setNumberDecimalSeparator(char value)
```


For the description of this property, please see [getNumberDecimalSeparator()](../../com.aspose.cells/workbooksettings\#getNumberDecimalSeparator--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | char |  |

### setNumberGroupSeparator(char value) {#setNumberGroupSeparator-char-}
```
public void setNumberGroupSeparator(char value)
```


For the description of this property, please see [getNumberGroupSeparator()](../../com.aspose.cells/workbooksettings\#getNumberGroupSeparator--)

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
| pageOrientationType | int | The [PageOrientationType](../../com.aspose.cells/pageorientationtype) |

### setPaperSize(int value) {#setPaperSize-int-}
```
public void setPaperSize(int value)
```


For the description of this property, please see [getPaperSize()](../../com.aspose.cells/workbooksettings\#getPaperSize--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setParsingFormulaOnOpen(boolean value) {#setParsingFormulaOnOpen-boolean-}
```
public void setParsingFormulaOnOpen(boolean value)
```


For the description of this property, please see [getParsingFormulaOnOpen()](../../com.aspose.cells/workbooksettings\#getParsingFormulaOnOpen--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


For the description of this property, please see [getPassword()](../../com.aspose.cells/workbooksettings\#getPassword--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setPrecisionAsDisplayed(boolean value) {#setPrecisionAsDisplayed-boolean-}
```
public void setPrecisionAsDisplayed(boolean value)
```


For the description of this property, please see [getPrecisionAsDisplayed()](../../com.aspose.cells/workbooksettings\#getPrecisionAsDisplayed--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setQuotePrefixToStyle(boolean value) {#setQuotePrefixToStyle-boolean-}
```
public void setQuotePrefixToStyle(boolean value)
```


For the description of this property, please see [getQuotePrefixToStyle()](../../com.aspose.cells/workbooksettings\#getQuotePrefixToStyle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setReCalculateOnOpen(boolean value) {#setReCalculateOnOpen-boolean-}
```
public void setReCalculateOnOpen(boolean value)
```


For the description of this property, please see [getReCalculateOnOpen()](../../com.aspose.cells/workbooksettings\#getReCalculateOnOpen--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setRecalculateBeforeSave(boolean value) {#setRecalculateBeforeSave-boolean-}
```
public void setRecalculateBeforeSave(boolean value)
```


For the description of this property, please see [getRecalculateBeforeSave()](../../com.aspose.cells/workbooksettings\#getRecalculateBeforeSave--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setRegion(int value) {#setRegion-int-}
```
public void setRegion(int value)
```


For the description of this property, please see [getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setRemovePersonalInformation(boolean value) {#setRemovePersonalInformation-boolean-}
```
public void setRemovePersonalInformation(boolean value)
```


For the description of this property, please see [getRemovePersonalInformation()](../../com.aspose.cells/workbooksettings\#getRemovePersonalInformation--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setRepairLoad(boolean value) {#setRepairLoad-boolean-}
```
public void setRepairLoad(boolean value)
```


For the description of this property, please see [getRepairLoad()](../../com.aspose.cells/workbooksettings\#getRepairLoad--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setResourceProvider(IStreamProvider value) {#setResourceProvider-com.aspose.cells.IStreamProvider-}
```
public void setResourceProvider(IStreamProvider value)
```


For the description of this property, please see [getResourceProvider()](../../com.aspose.cells/workbooksettings\#getResourceProvider--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setShared(boolean value) {#setShared-boolean-}
```
public void setShared(boolean value)
```


For the description of this property, please see [getShared()](../../com.aspose.cells/workbooksettings\#getShared--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSheetTabBarWidth(int value) {#setSheetTabBarWidth-int-}
```
public void setSheetTabBarWidth(int value)
```


For the description of this property, please see [getSheetTabBarWidth()](../../com.aspose.cells/workbooksettings\#getSheetTabBarWidth--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setShowTabs(boolean value) {#setShowTabs-boolean-}
```
public void setShowTabs(boolean value)
```


For the description of this property, please see [getShowTabs()](../../com.aspose.cells/workbooksettings\#getShowTabs--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSignificantDigits(int value) {#setSignificantDigits-int-}
```
public void setSignificantDigits(int value)
```


For the description of this property, please see [getSignificantDigits()](../../com.aspose.cells/workbooksettings\#getSignificantDigits--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


For the description of this property, please see [getStreamProvider()](../../com.aspose.cells/workbooksettings\#getStreamProvider--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setUpdateAdjacentCellsBorder(boolean value) {#setUpdateAdjacentCellsBorder-boolean-}
```
public void setUpdateAdjacentCellsBorder(boolean value)
```


For the description of this property, please see [getUpdateAdjacentCellsBorder()](../../com.aspose.cells/workbooksettings\#getUpdateAdjacentCellsBorder--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setUpdateLinksType(int value) {#setUpdateLinksType-int-}
```
public void setUpdateLinksType(int value)
```


For the description of this property, please see [getUpdateLinksType()](../../com.aspose.cells/workbooksettings\#getUpdateLinksType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setVScrollBarVisible(boolean value) {#setVScrollBarVisible-boolean-}
```
public void setVScrollBarVisible(boolean value)
```


For the description of this property, please see [isVScrollBarVisible()](../../com.aspose.cells/workbooksettings\#isVScrollBarVisible--)

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

### setWindowHeight(double value) {#setWindowHeight-double-}
```
public void setWindowHeight(double value)
```


For the description of this property, please see [getWindowHeight()](../../com.aspose.cells/workbooksettings\#getWindowHeight--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWindowHeightCM(double value) {#setWindowHeightCM-double-}
```
public void setWindowHeightCM(double value)
```


For the description of this property, please see [getWindowHeightCM()](../../com.aspose.cells/workbooksettings\#getWindowHeightCM--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWindowHeightInch(double value) {#setWindowHeightInch-double-}
```
public void setWindowHeightInch(double value)
```


For the description of this property, please see [getWindowHeightInch()](../../com.aspose.cells/workbooksettings\#getWindowHeightInch--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWindowLeft(double value) {#setWindowLeft-double-}
```
public void setWindowLeft(double value)
```


For the description of this property, please see [getWindowLeft()](../../com.aspose.cells/workbooksettings\#getWindowLeft--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWindowLeftCM(double value) {#setWindowLeftCM-double-}
```
public void setWindowLeftCM(double value)
```


For the description of this property, please see [getWindowLeftCM()](../../com.aspose.cells/workbooksettings\#getWindowLeftCM--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWindowLeftInch(double value) {#setWindowLeftInch-double-}
```
public void setWindowLeftInch(double value)
```


For the description of this property, please see [getWindowLeftInch()](../../com.aspose.cells/workbooksettings\#getWindowLeftInch--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWindowTop(double value) {#setWindowTop-double-}
```
public void setWindowTop(double value)
```


For the description of this property, please see [getWindowTop()](../../com.aspose.cells/workbooksettings\#getWindowTop--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWindowTopCM(double value) {#setWindowTopCM-double-}
```
public void setWindowTopCM(double value)
```


For the description of this property, please see [getWindowTopCM()](../../com.aspose.cells/workbooksettings\#getWindowTopCM--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWindowTopInch(double value) {#setWindowTopInch-double-}
```
public void setWindowTopInch(double value)
```


For the description of this property, please see [getWindowTopInch()](../../com.aspose.cells/workbooksettings\#getWindowTopInch--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWindowWidth(double value) {#setWindowWidth-double-}
```
public void setWindowWidth(double value)
```


For the description of this property, please see [getWindowWidth()](../../com.aspose.cells/workbooksettings\#getWindowWidth--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWindowWidthCM(double value) {#setWindowWidthCM-double-}
```
public void setWindowWidthCM(double value)
```


For the description of this property, please see [getWindowWidthCM()](../../com.aspose.cells/workbooksettings\#getWindowWidthCM--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWindowWidthInch(double value) {#setWindowWidthInch-double-}
```
public void setWindowWidthInch(double value)
```


For the description of this property, please see [getWindowWidthInch()](../../com.aspose.cells/workbooksettings\#getWindowWidthInch--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

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

