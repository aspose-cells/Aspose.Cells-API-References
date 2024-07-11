---
title: WorkbookSettings
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents all settings of the workbook.
type: docs
url: /nodejs-cpp/workbooksettings/
---

## WorkbookSettings class

Represents all settings of the workbook.

```javascript
class WorkbookSettings;
```


## Methods

| Method | Description |
| --- | --- |
| [getAuthor()](#getAuthor--)| Gets and sets the author of the file. |
| [setAuthor(string)](#setAuthor-string-)| Gets and sets the author of the file. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--)| Indicates whether checking custom number format when setting Style.Custom. |
| [setCheckCustomNumberFormat(boolean)](#setCheckCustomNumberFormat-boolean-)| Indicates whether checking custom number format when setting Style.Custom. |
| [getEnableMacros()](#getEnableMacros--)| Enable macros; |
| [setEnableMacros(boolean)](#setEnableMacros-boolean-)| Enable macros; |
| [getDate1904()](#getDate1904--)| Gets or sets a value which represents if the workbook uses the 1904 date system. |
| [setDate1904(boolean)](#setDate1904-boolean-)| Gets or sets a value which represents if the workbook uses the 1904 date system. |
| [getProtectionType()](#getProtectionType--)| Gets the protection type of the workbook. |
| [getDisplayDrawingObjects()](#getDisplayDrawingObjects--)| Indicates whether and how to show objects in the workbook. |
| [setDisplayDrawingObjects(DisplayDrawingObjects)](#setDisplayDrawingObjects-displaydrawingobjects-)| Indicates whether and how to show objects in the workbook. |
| [getSheetTabBarWidth()](#getSheetTabBarWidth--)| Width of worksheet tab bar (in 1/1000 of window width). |
| [setSheetTabBarWidth(number)](#setSheetTabBarWidth-number-)| Width of worksheet tab bar (in 1/1000 of window width). |
| [getShowTabs()](#getShowTabs--)| Get or sets a value whether the Workbook tabs are displayed. |
| [setShowTabs(boolean)](#setShowTabs-boolean-)| Get or sets a value whether the Workbook tabs are displayed. |
| [getFirstVisibleTab()](#getFirstVisibleTab--)| Gets or sets the first visible worksheet tab. |
| [setFirstVisibleTab(number)](#setFirstVisibleTab-number-)| Gets or sets the first visible worksheet tab. |
| [isHScrollBarVisible()](#isHScrollBarVisible--)| Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar. |
| [setIsHScrollBarVisible(boolean)](#setIsHScrollBarVisible-boolean-)| Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar. |
| [isVScrollBarVisible()](#isVScrollBarVisible--)| Gets or sets a value indicating whether the generated spreadsheet will contain a vertical scroll bar. |
| [setIsVScrollBarVisible(boolean)](#setIsVScrollBarVisible-boolean-)| Gets or sets a value indicating whether the generated spreadsheet will contain a vertical scroll bar. |
| [getShared()](#getShared--)| Gets or sets a value that indicates whether the Workbook is shared. |
| [setShared(boolean)](#setShared-boolean-)| Gets or sets a value that indicates whether the Workbook is shared. |
| [getLanguageCode()](#getLanguageCode--)| Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [setLanguageCode(CountryCode)](#setLanguageCode-countrycode-)| Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [getRegion()](#getRegion--)| Gets or sets the regional settings for workbook. |
| [setRegion(CountryCode)](#setRegion-countrycode-)| Gets or sets the regional settings for workbook. |
| [getGlobalizationSettings()](#getGlobalizationSettings--)| Gets and sets the globalization settings. |
| [setGlobalizationSettings(GlobalizationSettings)](#setGlobalizationSettings-globalizationsettings-)| Gets and sets the globalization settings. |
| [getNumberDecimalSeparator()](#getNumberDecimalSeparator--)| Gets or sets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Region. |
| [setNumberDecimalSeparator(string)](#setNumberDecimalSeparator-string-)| Gets or sets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Region. |
| [getNumberGroupSeparator()](#getNumberGroupSeparator--)| Gets or sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the group separator of current Region. |
| [setNumberGroupSeparator(string)](#setNumberGroupSeparator-string-)| Gets or sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the group separator of current Region. |
| [getPassword()](#getPassword--)| Represents Workbook file encryption password. |
| [setPassword(string)](#setPassword-string-)| Represents Workbook file encryption password. |
| [getWriteProtection()](#getWriteProtection--)| Provides access to the workbook write protection options. |
| [isEncrypted()](#isEncrypted--)| Gets a value that indicates whether a password is required to open this workbook. |
| [isProtected()](#isProtected--)| Gets a value that indicates whether the structure or window of the Workbook is protected. |
| [isDefaultEncrypted()](#isDefaultEncrypted--)| Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked. |
| [setIsDefaultEncrypted(boolean)](#setIsDefaultEncrypted-boolean-)| Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked. |
| [isMinimized()](#isMinimized--)| Represents whether the generated spreadsheet will be opened Minimized. |
| [setIsMinimized(boolean)](#setIsMinimized-boolean-)| Represents whether the generated spreadsheet will be opened Minimized. |
| [isHidden()](#isHidden--)| Indicates whether this workbook is hidden. |
| [setIsHidden(boolean)](#setIsHidden-boolean-)| Indicates whether this workbook is hidden. |
| [getAutoCompressPictures()](#getAutoCompressPictures--)| Specifies a boolean value that indicates the application automatically compressed pictures in the workbook. |
| [setAutoCompressPictures(boolean)](#setAutoCompressPictures-boolean-)| Specifies a boolean value that indicates the application automatically compressed pictures in the workbook. |
| [getRemovePersonalInformation()](#getRemovePersonalInformation--)| True if personal information can be removed from the specified workbook. |
| [setRemovePersonalInformation(boolean)](#setRemovePersonalInformation-boolean-)| True if personal information can be removed from the specified workbook. |
| [getHidePivotFieldList()](#getHidePivotFieldList--)| Gets and sets whether hide the field list for the PivotTable. |
| [setHidePivotFieldList(boolean)](#setHidePivotFieldList-boolean-)| Gets and sets whether hide the field list for the PivotTable. |
| [getUpdateLinksType()](#getUpdateLinksType--)| Gets and sets how updates external links when the workbook is opened. |
| [setUpdateLinksType(UpdateLinksType)](#setUpdateLinksType-updatelinkstype-)| Gets and sets how updates external links when the workbook is opened. |
| [getMaxRow()](#getMaxRow--)| Gets the max row index, zero-based. |
| [getMaxColumn()](#getMaxColumn--)| Gets the max column index, zero-based. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--)| Gets the settings for default values of style-related properties for this workbook. |
| [getWindowLeft()](#getWindowLeft--)| The distance from the left edge of the client area to the left edge of the window, in unit of point. |
| [setWindowLeft(number)](#setWindowLeft-number-)| The distance from the left edge of the client area to the left edge of the window, in unit of point. |
| [getWindowLeftInch()](#getWindowLeftInch--)| The distance from the left edge of the client area to the left edge of the window. In unit of inch. |
| [setWindowLeftInch(number)](#setWindowLeftInch-number-)| The distance from the left edge of the client area to the left edge of the window. In unit of inch. |
| [getWindowLeftCM()](#getWindowLeftCM--)| The distance from the left edge of the client area to the left edge of the window. In unit of centimeter. |
| [setWindowLeftCM(number)](#setWindowLeftCM-number-)| The distance from the left edge of the client area to the left edge of the window. In unit of centimeter. |
| [getWindowTop()](#getWindowTop--)| The distance from the top edge of the client area to the top edge of the window, in unit of point. |
| [setWindowTop(number)](#setWindowTop-number-)| The distance from the top edge of the client area to the top edge of the window, in unit of point. |
| [getWindowTopInch()](#getWindowTopInch--)| The distance from the top edge of the client area to the top edge of the window, in unit of inch. |
| [setWindowTopInch(number)](#setWindowTopInch-number-)| The distance from the top edge of the client area to the top edge of the window, in unit of inch. |
| [getWindowTopCM()](#getWindowTopCM--)| The distance from the top edge of the client area to the top edge of the window, in unit of centimeter. |
| [setWindowTopCM(number)](#setWindowTopCM-number-)| The distance from the top edge of the client area to the top edge of the window, in unit of centimeter. |
| [getWindowWidth()](#getWindowWidth--)| The width of the window, in unit of point. |
| [setWindowWidth(number)](#setWindowWidth-number-)| The width of the window, in unit of point. |
| [getWindowWidthInch()](#getWindowWidthInch--)| The width of the window, in unit of inch. |
| [setWindowWidthInch(number)](#setWindowWidthInch-number-)| The width of the window, in unit of inch. |
| [getWindowWidthCM()](#getWindowWidthCM--)| The width of the window, in unit of centimeter. |
| [setWindowWidthCM(number)](#setWindowWidthCM-number-)| The width of the window, in unit of centimeter. |
| [getWindowHeight()](#getWindowHeight--)| The height of the window, in unit of point. |
| [setWindowHeight(number)](#setWindowHeight-number-)| The height of the window, in unit of point. |
| [getWindowHeightInch()](#getWindowHeightInch--)| The height of the window, in unit of inch. |
| [setWindowHeightInch(number)](#setWindowHeightInch-number-)| The height of the window, in unit of inch. |
| [getWindowHeightCM()](#getWindowHeightCM--)| The height of the window, in unit of centimeter. |
| [setWindowHeightCM(number)](#setWindowHeightCM-number-)| The height of the window, in unit of centimeter. |
| [getUpdateAdjacentCellsBorder()](#getUpdateAdjacentCellsBorder--)| Indicates whether update adjacent cells' border. |
| [setUpdateAdjacentCellsBorder(boolean)](#setUpdateAdjacentCellsBorder-boolean-)| Indicates whether update adjacent cells' border. |
| [getSignificantDigits()](#getSignificantDigits--)| Gets and sets the number of significant digits. The default value is [CellsHelper.SignificantDigits](./cellshelper.significantdigits/). |
| [setSignificantDigits(number)](#setSignificantDigits-number-)| Gets and sets the number of significant digits. The default value is [CellsHelper.SignificantDigits](./cellshelper.significantdigits/). |
| [getCheckCompatibility()](#getCheckCompatibility--)| Indicates whether check compatibility with earlier versions when saving workbook. |
| [setCheckCompatibility(boolean)](#setCheckCompatibility-boolean-)| Indicates whether check compatibility with earlier versions when saving workbook. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--)| Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [setCheckExcelRestriction(boolean)](#setCheckExcelRestriction-boolean-)| Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [getAutoRecover()](#getAutoRecover--)| Indicates whether the file is marked for auto-recovery. |
| [setAutoRecover(boolean)](#setAutoRecover-boolean-)| Indicates whether the file is marked for auto-recovery. |
| [getCrashSave()](#getCrashSave--)| indicates whether the application last saved the workbook file after a crash. |
| [setCrashSave(boolean)](#setCrashSave-boolean-)| indicates whether the application last saved the workbook file after a crash. |
| [getDataExtractLoad()](#getDataExtractLoad--)| indicates whether the application last opened the workbook for data recovery. |
| [setDataExtractLoad(boolean)](#setDataExtractLoad-boolean-)| indicates whether the application last opened the workbook for data recovery. |
| [getRepairLoad()](#getRepairLoad--)| Indicates whether the application last opened the workbook in safe or repair mode. |
| [setRepairLoad(boolean)](#setRepairLoad-boolean-)| Indicates whether the application last opened the workbook in safe or repair mode. |
| [getBuildVersion()](#getBuildVersion--)| Specifies the incremental public release of the application. |
| [setBuildVersion(string)](#setBuildVersion-string-)| Specifies the incremental public release of the application. |
| [getMemorySetting()](#getMemorySetting--)| Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets. |
| [setMemorySetting(MemorySetting)](#setMemorySetting-memorysetting-)| Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets. |
| [getPaperSize()](#getPaperSize--)| Gets and sets the default print paper size. |
| [setPaperSize(PaperSizeType)](#setPaperSize-papersizetype-)| Gets and sets the default print paper size. |
| [setWarningCallback(IWarningCallback)](#setWarningCallback-iwarningcallback-)| Gets or sets warning callback. |
| [getWarningCallback()](#getWarningCallback--)| Gets or sets warning callback. |
| [getMaxRowsOfSharedFormula()](#getMaxRowsOfSharedFormula--)| Gets and sets the max row number of shared formula. |
| [setMaxRowsOfSharedFormula(number)](#setMaxRowsOfSharedFormula-number-)| Gets and sets the max row number of shared formula. |
| [getCompliance()](#getCompliance--)| Specifies the OOXML version for the output document. The default value is Ecma376_2006. |
| [setCompliance(OoxmlCompliance)](#setCompliance-ooxmlcompliance-)| Specifies the OOXML version for the output document. The default value is Ecma376_2006. |
| [getQuotePrefixToStyle()](#getQuotePrefixToStyle--)| Indicates whether setting [Style.QuotePrefix](./style.quoteprefix/) property when entering the string value(which starts  with single quote mark ) to the cell |
| [setQuotePrefixToStyle(boolean)](#setQuotePrefixToStyle-boolean-)| Indicates whether setting [Style.QuotePrefix](./style.quoteprefix/) property when entering the string value(which starts  with single quote mark ) to the cell |
| [getFormulaSettings()](#getFormulaSettings--)| Gets the settings for formula-related features. |
| [dispose()](#dispose--)| Releases resources. |
| [getThemeFont(FontSchemeType)](#getThemeFont-fontschemetype-)| Gets the default theme font name. |
| [setPageOrientationType(PageOrientationType)](#setPageOrientationType-pageorientationtype-)| Set the type of  print orientation for the whole workbook. |


### getAuthor() {#getAuthor--}

Gets and sets the author of the file.

```javascript
getAuthor() : string;
```


**Remarks**

It''s not set, check  [BuiltInDocumentPropertyCollection.Author](./builtindocumentpropertycollection.author/) first, then check the user of Environment.

### setAuthor(string) {#setAuthor-string-}

Gets and sets the author of the file.

```javascript
setAuthor(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

It''s not set, check  [BuiltInDocumentPropertyCollection.Author](./builtindocumentpropertycollection.author/) first, then check the user of Environment.

### getCheckCustomNumberFormat() {#getCheckCustomNumberFormat--}

Indicates whether checking custom number format when setting Style.Custom.

```javascript
getCheckCustomNumberFormat() : boolean;
```


### setCheckCustomNumberFormat(boolean) {#setCheckCustomNumberFormat-boolean-}

Indicates whether checking custom number format when setting Style.Custom.

```javascript
setCheckCustomNumberFormat(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getEnableMacros() {#getEnableMacros--}

Enable macros;

```javascript
getEnableMacros() : boolean;
```


**Remarks**

Now it only works when copying a worksheet to other worksheet in a workbook.

### setEnableMacros(boolean) {#setEnableMacros-boolean-}

Enable macros;

```javascript
setEnableMacros(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Now it only works when copying a worksheet to other worksheet in a workbook.

### getDate1904() {#getDate1904--}

Gets or sets a value which represents if the workbook uses the 1904 date system.

```javascript
getDate1904() : boolean;
```


### setDate1904(boolean) {#setDate1904-boolean-}

Gets or sets a value which represents if the workbook uses the 1904 date system.

```javascript
setDate1904(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getProtectionType() {#getProtectionType--}

Gets the protection type of the workbook.

```javascript
getProtectionType() : ProtectionType;
```


**Returns**

[ProtectionType](./protectiontype/)

### getDisplayDrawingObjects() {#getDisplayDrawingObjects--}

Indicates whether and how to show objects in the workbook.

```javascript
getDisplayDrawingObjects() : DisplayDrawingObjects;
```


**Returns**

[DisplayDrawingObjects](./displaydrawingobjects/)

### setDisplayDrawingObjects(DisplayDrawingObjects) {#setDisplayDrawingObjects-displaydrawingobjects-}

Indicates whether and how to show objects in the workbook.

```javascript
setDisplayDrawingObjects(value: DisplayDrawingObjects) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DisplayDrawingObjects](./displaydrawingobjects/) | The value to set. |

### getSheetTabBarWidth() {#getSheetTabBarWidth--}

Width of worksheet tab bar (in 1/1000 of window width).

```javascript
getSheetTabBarWidth() : number;
```


### setSheetTabBarWidth(number) {#setSheetTabBarWidth-number-}

Width of worksheet tab bar (in 1/1000 of window width).

```javascript
setSheetTabBarWidth(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getShowTabs() {#getShowTabs--}

Get or sets a value whether the Workbook tabs are displayed.

```javascript
getShowTabs() : boolean;
```


**Remarks**

The default value is true.

### setShowTabs(boolean) {#setShowTabs-boolean-}

Get or sets a value whether the Workbook tabs are displayed.

```javascript
setShowTabs(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is true.

### getFirstVisibleTab() {#getFirstVisibleTab--}

Gets or sets the first visible worksheet tab.

```javascript
getFirstVisibleTab() : number;
```


### setFirstVisibleTab(number) {#setFirstVisibleTab-number-}

Gets or sets the first visible worksheet tab.

```javascript
setFirstVisibleTab(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### isHScrollBarVisible() {#isHScrollBarVisible--}

Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar.

```javascript
isHScrollBarVisible() : boolean;
```


**Remarks**

The default value is true.

### setIsHScrollBarVisible(boolean) {#setIsHScrollBarVisible-boolean-}

Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar.

```javascript
setIsHScrollBarVisible(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is true.

### isVScrollBarVisible() {#isVScrollBarVisible--}

Gets or sets a value indicating whether the generated spreadsheet will contain a vertical scroll bar.

```javascript
isVScrollBarVisible() : boolean;
```


**Remarks**

The default value is true.

### setIsVScrollBarVisible(boolean) {#setIsVScrollBarVisible-boolean-}

Gets or sets a value indicating whether the generated spreadsheet will contain a vertical scroll bar.

```javascript
setIsVScrollBarVisible(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is true.

### getShared() {#getShared--}

Gets or sets a value that indicates whether the Workbook is shared.

```javascript
getShared() : boolean;
```


**Remarks**

The default value is false.

### setShared(boolean) {#setShared-boolean-}

Gets or sets a value that indicates whether the Workbook is shared.

```javascript
setShared(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is false.

### getLanguageCode() {#getLanguageCode--}

Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file.

```javascript
getLanguageCode() : CountryCode;
```


**Returns**

[CountryCode](./countrycode/)

### setLanguageCode(CountryCode) {#setLanguageCode-countrycode-}

Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file.

```javascript
setLanguageCode(value: CountryCode) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CountryCode](./countrycode/) | The value to set. |

### getRegion() {#getRegion--}

Gets or sets the regional settings for workbook.

```javascript
getRegion() : CountryCode;
```


**Returns**

[CountryCode](./countrycode/)

**Remarks**

1. Regional settings used by Aspose.Cells component for a workbook loaded from template file: i). For an XLS file, there are fields defined for regional settings and MS Excel does save regional settings data into the file when saving the XLS file. So, we use the saved region in the template file for the workbook. If you do not want to use the region saved in the XLS file, please reset it to the expected one (such as, CountryCode.Default) after loading the template file. And, we save the user specified value (by this method) into the file too when saving an XLS file. ii). For other file formats, such as, XLSX, XLSB...etc., there is no field defined for regional settings in the file format specification. So, we use the regional settings of application's environment for the workbook. And, the user specified value (by this method) cannot be kept for the generated files with those file formats. 2. For the view effect in MS Excel: The applied regional settings here can take effect only at runtime with Aspose.Cells component and not when viewing the generated file with MS Excel. Even for the generated XLS file in which the specified regional settings data has been saved, when viewing/editing it with MS Excel, the used region to perform formatting by MS Excel is always the default regional settings of the environment where MS Excel is running, not the one saved in the file. It is MS Excel's behavior and cannot be changed by code.

### setRegion(CountryCode) {#setRegion-countrycode-}

Gets or sets the regional settings for workbook.

```javascript
setRegion(value: CountryCode) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CountryCode](./countrycode/) | The value to set. |

**Remarks**

1. Regional settings used by Aspose.Cells component for a workbook loaded from template file: i). For an XLS file, there are fields defined for regional settings and MS Excel does save regional settings data into the file when saving the XLS file. So, we use the saved region in the template file for the workbook. If you do not want to use the region saved in the XLS file, please reset it to the expected one (such as, CountryCode.Default) after loading the template file. And, we save the user specified value (by this method) into the file too when saving an XLS file. ii). For other file formats, such as, XLSX, XLSB...etc., there is no field defined for regional settings in the file format specification. So, we use the regional settings of application's environment for the workbook. And, the user specified value (by this method) cannot be kept for the generated files with those file formats. 2. For the view effect in MS Excel: The applied regional settings here can take effect only at runtime with Aspose.Cells component and not when viewing the generated file with MS Excel. Even for the generated XLS file in which the specified regional settings data has been saved, when viewing/editing it with MS Excel, the used region to perform formatting by MS Excel is always the default regional settings of the environment where MS Excel is running, not the one saved in the file. It is MS Excel's behavior and cannot be changed by code.

### getGlobalizationSettings() {#getGlobalizationSettings--}

Gets and sets the globalization settings.

```javascript
getGlobalizationSettings() : GlobalizationSettings;
```


**Returns**

[GlobalizationSettings](./globalizationsettings/)

### setGlobalizationSettings(GlobalizationSettings) {#setGlobalizationSettings-globalizationsettings-}

Gets and sets the globalization settings.

```javascript
setGlobalizationSettings(value: GlobalizationSettings) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GlobalizationSettings](./globalizationsettings/) | The value to set. |

### getNumberDecimalSeparator() {#getNumberDecimalSeparator--}

Gets or sets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Region.

```javascript
getNumberDecimalSeparator() : string;
```


### setNumberDecimalSeparator(string) {#setNumberDecimalSeparator-string-}

Gets or sets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Region.

```javascript
setNumberDecimalSeparator(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getNumberGroupSeparator() {#getNumberGroupSeparator--}

Gets or sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the group separator of current Region.

```javascript
getNumberGroupSeparator() : string;
```


### setNumberGroupSeparator(string) {#setNumberGroupSeparator-string-}

Gets or sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the group separator of current Region.

```javascript
setNumberGroupSeparator(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getPassword() {#getPassword--}

Represents Workbook file encryption password.

```javascript
getPassword() : string;
```


### setPassword(string) {#setPassword-string-}

Represents Workbook file encryption password.

```javascript
setPassword(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getWriteProtection() {#getWriteProtection--}

Provides access to the workbook write protection options.

```javascript
getWriteProtection() : WriteProtection;
```


**Returns**

[WriteProtection](./writeprotection/)

### isEncrypted() {#isEncrypted--}

Gets a value that indicates whether a password is required to open this workbook.

```javascript
isEncrypted() : boolean;
```


### isProtected() {#isProtected--}

Gets a value that indicates whether the structure or window of the Workbook is protected.

```javascript
isProtected() : boolean;
```


### isDefaultEncrypted() {#isDefaultEncrypted--}

Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked.

```javascript
isDefaultEncrypted() : boolean;
```


**Remarks**

The default value is false now. It's same as MS Excel 2013.

### setIsDefaultEncrypted(boolean) {#setIsDefaultEncrypted-boolean-}

Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked.

```javascript
setIsDefaultEncrypted(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is false now. It's same as MS Excel 2013.

### isMinimized() {#isMinimized--}

Represents whether the generated spreadsheet will be opened Minimized.

```javascript
isMinimized() : boolean;
```


### setIsMinimized(boolean) {#setIsMinimized-boolean-}

Represents whether the generated spreadsheet will be opened Minimized.

```javascript
setIsMinimized(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isHidden() {#isHidden--}

Indicates whether this workbook is hidden.

```javascript
isHidden() : boolean;
```


### setIsHidden(boolean) {#setIsHidden-boolean-}

Indicates whether this workbook is hidden.

```javascript
setIsHidden(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAutoCompressPictures() {#getAutoCompressPictures--}

Specifies a boolean value that indicates the application automatically compressed pictures in the workbook.

```javascript
getAutoCompressPictures() : boolean;
```


### setAutoCompressPictures(boolean) {#setAutoCompressPictures-boolean-}

Specifies a boolean value that indicates the application automatically compressed pictures in the workbook.

```javascript
setAutoCompressPictures(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getRemovePersonalInformation() {#getRemovePersonalInformation--}

True if personal information can be removed from the specified workbook.

```javascript
getRemovePersonalInformation() : boolean;
```


### setRemovePersonalInformation(boolean) {#setRemovePersonalInformation-boolean-}

True if personal information can be removed from the specified workbook.

```javascript
setRemovePersonalInformation(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getHidePivotFieldList() {#getHidePivotFieldList--}

Gets and sets whether hide the field list for the PivotTable.

```javascript
getHidePivotFieldList() : boolean;
```


### setHidePivotFieldList(boolean) {#setHidePivotFieldList-boolean-}

Gets and sets whether hide the field list for the PivotTable.

```javascript
setHidePivotFieldList(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getUpdateLinksType() {#getUpdateLinksType--}

Gets and sets how updates external links when the workbook is opened.

```javascript
getUpdateLinksType() : UpdateLinksType;
```


**Returns**

[UpdateLinksType](./updatelinkstype/)

### setUpdateLinksType(UpdateLinksType) {#setUpdateLinksType-updatelinkstype-}

Gets and sets how updates external links when the workbook is opened.

```javascript
setUpdateLinksType(value: UpdateLinksType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [UpdateLinksType](./updatelinkstype/) | The value to set. |

### getMaxRow() {#getMaxRow--}

Gets the max row index, zero-based.

```javascript
getMaxRow() : number;
```


**Remarks**

Returns 65535 if the file format is Excel97-2003;

### getMaxColumn() {#getMaxColumn--}

Gets the max column index, zero-based.

```javascript
getMaxColumn() : number;
```


**Remarks**

Returns 255 if the file format is Excel97-2003;

### getDefaultStyleSettings() {#getDefaultStyleSettings--}

Gets the settings for default values of style-related properties for this workbook.

```javascript
getDefaultStyleSettings() : DefaultStyleSettings;
```


**Returns**

[DefaultStyleSettings](./defaultstylesettings/)

### getWindowLeft() {#getWindowLeft--}

The distance from the left edge of the client area to the left edge of the window, in unit of point.

```javascript
getWindowLeft() : number;
```


### setWindowLeft(number) {#setWindowLeft-number-}

The distance from the left edge of the client area to the left edge of the window, in unit of point.

```javascript
setWindowLeft(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWindowLeftInch() {#getWindowLeftInch--}

The distance from the left edge of the client area to the left edge of the window. In unit of inch.

```javascript
getWindowLeftInch() : number;
```


### setWindowLeftInch(number) {#setWindowLeftInch-number-}

The distance from the left edge of the client area to the left edge of the window. In unit of inch.

```javascript
setWindowLeftInch(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWindowLeftCM() {#getWindowLeftCM--}

The distance from the left edge of the client area to the left edge of the window. In unit of centimeter.

```javascript
getWindowLeftCM() : number;
```


### setWindowLeftCM(number) {#setWindowLeftCM-number-}

The distance from the left edge of the client area to the left edge of the window. In unit of centimeter.

```javascript
setWindowLeftCM(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWindowTop() {#getWindowTop--}

The distance from the top edge of the client area to the top edge of the window, in unit of point.

```javascript
getWindowTop() : number;
```


### setWindowTop(number) {#setWindowTop-number-}

The distance from the top edge of the client area to the top edge of the window, in unit of point.

```javascript
setWindowTop(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWindowTopInch() {#getWindowTopInch--}

The distance from the top edge of the client area to the top edge of the window, in unit of inch.

```javascript
getWindowTopInch() : number;
```


### setWindowTopInch(number) {#setWindowTopInch-number-}

The distance from the top edge of the client area to the top edge of the window, in unit of inch.

```javascript
setWindowTopInch(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWindowTopCM() {#getWindowTopCM--}

The distance from the top edge of the client area to the top edge of the window, in unit of centimeter.

```javascript
getWindowTopCM() : number;
```


### setWindowTopCM(number) {#setWindowTopCM-number-}

The distance from the top edge of the client area to the top edge of the window, in unit of centimeter.

```javascript
setWindowTopCM(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWindowWidth() {#getWindowWidth--}

The width of the window, in unit of point.

```javascript
getWindowWidth() : number;
```


### setWindowWidth(number) {#setWindowWidth-number-}

The width of the window, in unit of point.

```javascript
setWindowWidth(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWindowWidthInch() {#getWindowWidthInch--}

The width of the window, in unit of inch.

```javascript
getWindowWidthInch() : number;
```


### setWindowWidthInch(number) {#setWindowWidthInch-number-}

The width of the window, in unit of inch.

```javascript
setWindowWidthInch(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWindowWidthCM() {#getWindowWidthCM--}

The width of the window, in unit of centimeter.

```javascript
getWindowWidthCM() : number;
```


### setWindowWidthCM(number) {#setWindowWidthCM-number-}

The width of the window, in unit of centimeter.

```javascript
setWindowWidthCM(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWindowHeight() {#getWindowHeight--}

The height of the window, in unit of point.

```javascript
getWindowHeight() : number;
```


### setWindowHeight(number) {#setWindowHeight-number-}

The height of the window, in unit of point.

```javascript
setWindowHeight(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWindowHeightInch() {#getWindowHeightInch--}

The height of the window, in unit of inch.

```javascript
getWindowHeightInch() : number;
```


### setWindowHeightInch(number) {#setWindowHeightInch-number-}

The height of the window, in unit of inch.

```javascript
setWindowHeightInch(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWindowHeightCM() {#getWindowHeightCM--}

The height of the window, in unit of centimeter.

```javascript
getWindowHeightCM() : number;
```


### setWindowHeightCM(number) {#setWindowHeightCM-number-}

The height of the window, in unit of centimeter.

```javascript
setWindowHeightCM(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getUpdateAdjacentCellsBorder() {#getUpdateAdjacentCellsBorder--}

Indicates whether update adjacent cells' border.

```javascript
getUpdateAdjacentCellsBorder() : boolean;
```


**Remarks**

The default value is false. For example: the bottom border of the cell A1 is update, the top border of the cell A2 should be changed too.

### setUpdateAdjacentCellsBorder(boolean) {#setUpdateAdjacentCellsBorder-boolean-}

Indicates whether update adjacent cells' border.

```javascript
setUpdateAdjacentCellsBorder(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is false. For example: the bottom border of the cell A1 is update, the top border of the cell A2 should be changed too.

### getSignificantDigits() {#getSignificantDigits--}

Gets and sets the number of significant digits. The default value is [CellsHelper.SignificantDigits](./cellshelper.significantdigits/).

```javascript
getSignificantDigits() : number;
```


**Remarks**

Only could be 15 or 17 now.

### setSignificantDigits(number) {#setSignificantDigits-number-}

Gets and sets the number of significant digits. The default value is [CellsHelper.SignificantDigits](./cellshelper.significantdigits/).

```javascript
setSignificantDigits(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

Only could be 15 or 17 now.

### getCheckCompatibility() {#getCheckCompatibility--}

Indicates whether check compatibility with earlier versions when saving workbook.

```javascript
getCheckCompatibility() : boolean;
```


**Remarks**

The default value is true. Only for Excel97-2003 xls or xlt files.

### setCheckCompatibility(boolean) {#setCheckCompatibility-boolean-}

Indicates whether check compatibility with earlier versions when saving workbook.

```javascript
setCheckCompatibility(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is true. Only for Excel97-2003 xls or xlt files.

### getCheckExcelRestriction() {#getCheckExcelRestriction--}

Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.

```javascript
getCheckExcelRestriction() : boolean;
```


### setCheckExcelRestriction(boolean) {#setCheckExcelRestriction-boolean-}

Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.

```javascript
setCheckExcelRestriction(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAutoRecover() {#getAutoRecover--}

Indicates whether the file is marked for auto-recovery.

```javascript
getAutoRecover() : boolean;
```


### setAutoRecover(boolean) {#setAutoRecover-boolean-}

Indicates whether the file is marked for auto-recovery.

```javascript
setAutoRecover(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCrashSave() {#getCrashSave--}

indicates whether the application last saved the workbook file after a crash.

```javascript
getCrashSave() : boolean;
```


### setCrashSave(boolean) {#setCrashSave-boolean-}

indicates whether the application last saved the workbook file after a crash.

```javascript
setCrashSave(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getDataExtractLoad() {#getDataExtractLoad--}

indicates whether the application last opened the workbook for data recovery.

```javascript
getDataExtractLoad() : boolean;
```


### setDataExtractLoad(boolean) {#setDataExtractLoad-boolean-}

indicates whether the application last opened the workbook for data recovery.

```javascript
setDataExtractLoad(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getRepairLoad() {#getRepairLoad--}

Indicates whether the application last opened the workbook in safe or repair mode.

```javascript
getRepairLoad() : boolean;
```


### setRepairLoad(boolean) {#setRepairLoad-boolean-}

Indicates whether the application last opened the workbook in safe or repair mode.

```javascript
setRepairLoad(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getBuildVersion() {#getBuildVersion--}

Specifies the incremental public release of the application.

```javascript
getBuildVersion() : string;
```


### setBuildVersion(string) {#setBuildVersion-string-}

Specifies the incremental public release of the application.

```javascript
setBuildVersion(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getMemorySetting() {#getMemorySetting--}

Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets.

```javascript
getMemorySetting() : MemorySetting;
```


**Returns**

[MemorySetting](./memorysetting/)

### setMemorySetting(MemorySetting) {#setMemorySetting-memorysetting-}

Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets.

```javascript
setMemorySetting(value: MemorySetting) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MemorySetting](./memorysetting/) | The value to set. |

### getPaperSize() {#getPaperSize--}

Gets and sets the default print paper size.

```javascript
getPaperSize() : PaperSizeType;
```


**Returns**

[PaperSizeType](./papersizetype/)

**Remarks**

If there is no setting about paper size,MS Excel will use default printer's setting.

### setPaperSize(PaperSizeType) {#setPaperSize-papersizetype-}

Gets and sets the default print paper size.

```javascript
setPaperSize(value: PaperSizeType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PaperSizeType](./papersizetype/) | The value to set. |

**Remarks**

If there is no setting about paper size,MS Excel will use default printer's setting.

### setWarningCallback(IWarningCallback) {#setWarningCallback-iwarningcallback-}

Gets or sets warning callback.

```javascript
setWarningCallback(value: IWarningCallback) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IWarningCallback](./iwarningcallback/) | The value to set. |

### getWarningCallback() {#getWarningCallback--}

Gets or sets warning callback.

```javascript
getWarningCallback() : IWarningCallback;
```


**Returns**

[IWarningCallback](./iwarningcallback/)

### getMaxRowsOfSharedFormula() {#getMaxRowsOfSharedFormula--}

Gets and sets the max row number of shared formula.

```javascript
getMaxRowsOfSharedFormula() : number;
```


**Remarks**

If the number is too large, the autofilter works very slow in MS Excel 2013.

### setMaxRowsOfSharedFormula(number) {#setMaxRowsOfSharedFormula-number-}

Gets and sets the max row number of shared formula.

```javascript
setMaxRowsOfSharedFormula(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

If the number is too large, the autofilter works very slow in MS Excel 2013.

### getCompliance() {#getCompliance--}

Specifies the OOXML version for the output document. The default value is Ecma376_2006.

```javascript
getCompliance() : OoxmlCompliance;
```


**Returns**

[OoxmlCompliance](./ooxmlcompliance/)

**Remarks**

Only for .xlsx files.

### setCompliance(OoxmlCompliance) {#setCompliance-ooxmlcompliance-}

Specifies the OOXML version for the output document. The default value is Ecma376_2006.

```javascript
setCompliance(value: OoxmlCompliance) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [OoxmlCompliance](./ooxmlcompliance/) | The value to set. |

**Remarks**

Only for .xlsx files.

### getQuotePrefixToStyle() {#getQuotePrefixToStyle--}

Indicates whether setting [Style.QuotePrefix](./style.quoteprefix/) property when entering the string value(which starts  with single quote mark ) to the cell

```javascript
getQuotePrefixToStyle() : boolean;
```


### setQuotePrefixToStyle(boolean) {#setQuotePrefixToStyle-boolean-}

Indicates whether setting [Style.QuotePrefix](./style.quoteprefix/) property when entering the string value(which starts  with single quote mark ) to the cell

```javascript
setQuotePrefixToStyle(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getFormulaSettings() {#getFormulaSettings--}

Gets the settings for formula-related features.

```javascript
getFormulaSettings() : FormulaSettings;
```


**Returns**

[FormulaSettings](./formulasettings/)

### dispose() {#dispose--}

Releases resources.

```javascript
dispose() : void;
```


### getThemeFont(FontSchemeType) {#getThemeFont-fontschemetype-}

Gets the default theme font name.

```javascript
getThemeFont(type: FontSchemeType) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [FontSchemeType](./fontschemetype/) | The scheme type of the font. |

### setPageOrientationType(PageOrientationType) {#setPageOrientationType-pageorientationtype-}

Set the type of  print orientation for the whole workbook.

```javascript
setPageOrientationType(pageOrientationType: PageOrientationType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageOrientationType | [PageOrientationType](./pageorientationtype/) | The page orientation type |


