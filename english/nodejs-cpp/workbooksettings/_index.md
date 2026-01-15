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


## Properties

| Property | Type | Description |
| --- | --- | --- |
| [author](#author--)| string | Gets and sets the author of the file. |
| [checkCustomNumberFormat](#checkCustomNumberFormat--)| boolean | Indicates whether checking custom number format when setting Style.Custom. |
| [enableMacros](#enableMacros--)| boolean | Enable macros; |
| [date1904](#date1904--)| boolean | Gets or sets a value which represents if the workbook uses the 1904 date system. |
| [protectionType](#protectionType--)| ProtectionType | Readonly. Gets the protection type of the workbook. |
| [displayDrawingObjects](#displayDrawingObjects--)| DisplayDrawingObjects | Indicates whether and how to show objects in the workbook. |
| [sheetTabBarWidth](#sheetTabBarWidth--)| number | Width of worksheet tab bar (in 1/1000 of window width). |
| [showTabs](#showTabs--)| boolean | Get or sets a value whether the Workbook tabs are displayed. |
| [firstVisibleTab](#firstVisibleTab--)| number | Gets or sets the first visible worksheet tab. |
| [isHScrollBarVisible](#isHScrollBarVisible--)| boolean | Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar. |
| [isVScrollBarVisible](#isVScrollBarVisible--)| boolean | Gets or sets a value indicating whether the generated spreadsheet will contain a vertical scroll bar. |
| [shared](#shared--)| boolean | Gets or sets a value that indicates whether the Workbook is shared. |
| [languageCode](#languageCode--)| CountryCode | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [region](#region--)| CountryCode | Gets or sets the regional settings for workbook. |
| [globalizationSettings](#globalizationSettings--)| GlobalizationSettings | Gets and sets the globalization settings. |
| [numberDecimalSeparator](#numberDecimalSeparator--)| string | Gets or sets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Region. |
| [numberGroupSeparator](#numberGroupSeparator--)| string | Gets or sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the group separator of current Region. |
| [password](#password--)| string | Represents Workbook file encryption password. |
| [writeProtection](#writeProtection--)| WriteProtection | Readonly. Provides access to the workbook write protection options. |
| [isEncrypted](#isEncrypted--)| boolean | Readonly. Gets a value that indicates whether a password is required to open this workbook. |
| [isProtected](#isProtected--)| boolean | Readonly. Gets a value that indicates whether the structure or window of the Workbook is protected. |
| [isDefaultEncrypted](#isDefaultEncrypted--)| boolean | Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked. |
| [isMinimized](#isMinimized--)| boolean | Represents whether the generated spreadsheet will be opened Minimized. |
| [isHidden](#isHidden--)| boolean | Indicates whether this workbook is hidden. |
| [autoCompressPictures](#autoCompressPictures--)| boolean | Specifies a boolean value that indicates the application automatically compressed pictures in the workbook. |
| [removePersonalInformation](#removePersonalInformation--)| boolean | True if personal information can be removed from the specified workbook. |
| [hidePivotFieldList](#hidePivotFieldList--)| boolean | Gets and sets whether hide the field list for the PivotTable. |
| [maxUniqueItemsPerField](#maxUniqueItemsPerField--)| number | Gets and set the limitation of unique items per field |
| [updateLinksType](#updateLinksType--)| UpdateLinksType | Gets and sets how updates external links when the workbook is opened. |
| [maxRow](#maxRow--)| number | Readonly. Gets the max row index, zero-based. |
| [maxColumn](#maxColumn--)| number | Readonly. Gets the max column index, zero-based. |
| [smartTagOptions](#smartTagOptions--)| SmartTagOptions | Readonly. Gets the options of the smart tag. |
| [defaultStyleSettings](#defaultStyleSettings--)| DefaultStyleSettings | Readonly. Gets the settings for default values of style-related properties for this workbook. |
| [windowLeft](#windowLeft--)| number | The distance from the left edge of the client area to the left edge of the window, in unit of point. |
| [windowLeftInch](#windowLeftInch--)| number | The distance from the left edge of the client area to the left edge of the window. In unit of inch. |
| [windowLeftCM](#windowLeftCM--)| number | The distance from the left edge of the client area to the left edge of the window. In unit of centimeter. |
| [windowTop](#windowTop--)| number | The distance from the top edge of the client area to the top edge of the window, in unit of point. |
| [windowTopInch](#windowTopInch--)| number | The distance from the top edge of the client area to the top edge of the window, in unit of inch. |
| [windowTopCM](#windowTopCM--)| number | The distance from the top edge of the client area to the top edge of the window, in unit of centimeter. |
| [windowWidth](#windowWidth--)| number | The width of the window, in unit of point. |
| [windowWidthInch](#windowWidthInch--)| number | The width of the window, in unit of inch. |
| [windowWidthCM](#windowWidthCM--)| number | The width of the window, in unit of centimeter. |
| [windowHeight](#windowHeight--)| number | The height of the window, in unit of point. |
| [windowHeightInch](#windowHeightInch--)| number | The height of the window, in unit of inch. |
| [windowHeightCM](#windowHeightCM--)| number | The height of the window, in unit of centimeter. |
| [updateAdjacentCellsBorder](#updateAdjacentCellsBorder--)| boolean | Indicates whether update adjacent cells' border. |
| [significantDigitsType](#significantDigitsType--)| SignificantDigitsType | Gets and sets the type of significant digits for outputing numeric values in this workbook. Default value is [CellsHelper.SignificantDigitsType](../cellshelper.significantdigitstype/). |
| [checkCompatibility](#checkCompatibility--)| boolean | Indicates whether check compatibility with earlier versions when saving workbook. |
| [checkExcelRestriction](#checkExcelRestriction--)| boolean | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [autoRecover](#autoRecover--)| boolean | Indicates whether the file is marked for auto-recovery. |
| [crashSave](#crashSave--)| boolean | indicates whether the application last saved the workbook file after a crash. |
| [dataExtractLoad](#dataExtractLoad--)| boolean | indicates whether the application last opened the workbook for data recovery. |
| [repairLoad](#repairLoad--)| boolean | Indicates whether the application last opened the workbook in safe or repair mode. |
| [buildVersion](#buildVersion--)| string | Specifies the incremental public release of the application. |
| [memorySetting](#memorySetting--)| MemorySetting | Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets. |
| [paperSize](#paperSize--)| PaperSizeType | Gets and sets the default print paper size. |
| [warningCallback](#warningCallback--)| IWarningCallback | Gets or sets warning callback. |
| [maxRowsOfSharedFormula](#maxRowsOfSharedFormula--)| number | Gets and sets the max row number of shared formula. |
| [compliance](#compliance--)| OoxmlCompliance | Specifies the OOXML version for the output document. The default value is Ecma376_2006. |
| [quotePrefixToStyle](#quotePrefixToStyle--)| boolean | Indicates whether setting [Style.QuotePrefix](../style.quoteprefix/) property when entering the string value(which starts  with single quote mark ) to the cell |
| [formulaSettings](#formulaSettings--)| FormulaSettings | Readonly. Gets the settings for formula-related features. |
| [propertiesFollowChartPoint](#propertiesFollowChartPoint--)| boolean | Indicates whether datapoint properties and datalabels in all charts in this workbook follow their reference. |
| [discardImageEditData](#discardImageEditData--)| boolean | Indicates whether discarding editting image data. |
| [defaultImageResolution](#defaultImageResolution--)| number | Gets and sets default resolution of image. |
| [wpsCompatibility](#wpsCompatibility--)| boolean | Indicates whether to be compatible with WPS. |

## Methods

| Method | Description |
| --- | --- |
| [getAuthor()](#getAuthor--)| <b>@deprecated.</b> Please use the 'author' property instead. Gets and sets the author of the file. |
| [setAuthor(string)](#setAuthor-string-)| <b>@deprecated.</b> Please use the 'author' property instead. Gets and sets the author of the file. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--)| <b>@deprecated.</b> Please use the 'checkCustomNumberFormat' property instead. Indicates whether checking custom number format when setting Style.Custom. |
| [setCheckCustomNumberFormat(boolean)](#setCheckCustomNumberFormat-boolean-)| <b>@deprecated.</b> Please use the 'checkCustomNumberFormat' property instead. Indicates whether checking custom number format when setting Style.Custom. |
| [getEnableMacros()](#getEnableMacros--)| <b>@deprecated.</b> Please use the 'enableMacros' property instead. Enable macros; |
| [setEnableMacros(boolean)](#setEnableMacros-boolean-)| <b>@deprecated.</b> Please use the 'enableMacros' property instead. Enable macros; |
| [getDate1904()](#getDate1904--)| <b>@deprecated.</b> Please use the 'date1904' property instead. Gets or sets a value which represents if the workbook uses the 1904 date system. |
| [setDate1904(boolean)](#setDate1904-boolean-)| <b>@deprecated.</b> Please use the 'date1904' property instead. Gets or sets a value which represents if the workbook uses the 1904 date system. |
| [getProtectionType()](#getProtectionType--)| <b>@deprecated.</b> Please use the 'protectionType' property instead. Gets the protection type of the workbook. |
| [getDisplayDrawingObjects()](#getDisplayDrawingObjects--)| <b>@deprecated.</b> Please use the 'displayDrawingObjects' property instead. Indicates whether and how to show objects in the workbook. |
| [setDisplayDrawingObjects(DisplayDrawingObjects)](#setDisplayDrawingObjects-displaydrawingobjects-)| <b>@deprecated.</b> Please use the 'displayDrawingObjects' property instead. Indicates whether and how to show objects in the workbook. |
| [getSheetTabBarWidth()](#getSheetTabBarWidth--)| <b>@deprecated.</b> Please use the 'sheetTabBarWidth' property instead. Width of worksheet tab bar (in 1/1000 of window width). |
| [setSheetTabBarWidth(number)](#setSheetTabBarWidth-number-)| <b>@deprecated.</b> Please use the 'sheetTabBarWidth' property instead. Width of worksheet tab bar (in 1/1000 of window width). |
| [getShowTabs()](#getShowTabs--)| <b>@deprecated.</b> Please use the 'showTabs' property instead. Get or sets a value whether the Workbook tabs are displayed. |
| [setShowTabs(boolean)](#setShowTabs-boolean-)| <b>@deprecated.</b> Please use the 'showTabs' property instead. Get or sets a value whether the Workbook tabs are displayed. |
| [getFirstVisibleTab()](#getFirstVisibleTab--)| <b>@deprecated.</b> Please use the 'firstVisibleTab' property instead. Gets or sets the first visible worksheet tab. |
| [setFirstVisibleTab(number)](#setFirstVisibleTab-number-)| <b>@deprecated.</b> Please use the 'firstVisibleTab' property instead. Gets or sets the first visible worksheet tab. |
| [isHScrollBarVisible()](#isHScrollBarVisible--)| <b>@deprecated.</b> Please use the 'isHScrollBarVisible' property instead. Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar. |
| [setIsHScrollBarVisible(boolean)](#setIsHScrollBarVisible-boolean-)| <b>@deprecated.</b> Please use the 'isHScrollBarVisible' property instead. Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar. |
| [isVScrollBarVisible()](#isVScrollBarVisible--)| <b>@deprecated.</b> Please use the 'isVScrollBarVisible' property instead. Gets or sets a value indicating whether the generated spreadsheet will contain a vertical scroll bar. |
| [setIsVScrollBarVisible(boolean)](#setIsVScrollBarVisible-boolean-)| <b>@deprecated.</b> Please use the 'isVScrollBarVisible' property instead. Gets or sets a value indicating whether the generated spreadsheet will contain a vertical scroll bar. |
| [getShared()](#getShared--)| <b>@deprecated.</b> Please use the 'shared' property instead. Gets or sets a value that indicates whether the Workbook is shared. |
| [setShared(boolean)](#setShared-boolean-)| <b>@deprecated.</b> Please use the 'shared' property instead. Gets or sets a value that indicates whether the Workbook is shared. |
| [getLanguageCode()](#getLanguageCode--)| <b>@deprecated.</b> Please use the 'languageCode' property instead. Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [setLanguageCode(CountryCode)](#setLanguageCode-countrycode-)| <b>@deprecated.</b> Please use the 'languageCode' property instead. Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [getRegion()](#getRegion--)| <b>@deprecated.</b> Please use the 'region' property instead. Gets or sets the regional settings for workbook. |
| [setRegion(CountryCode)](#setRegion-countrycode-)| <b>@deprecated.</b> Please use the 'region' property instead. Gets or sets the regional settings for workbook. |
| [getGlobalizationSettings()](#getGlobalizationSettings--)| <b>@deprecated.</b> Please use the 'globalizationSettings' property instead. Gets and sets the globalization settings. |
| [setGlobalizationSettings(GlobalizationSettings)](#setGlobalizationSettings-globalizationsettings-)| <b>@deprecated.</b> Please use the 'globalizationSettings' property instead. Gets and sets the globalization settings. |
| [getNumberDecimalSeparator()](#getNumberDecimalSeparator--)| <b>@deprecated.</b> Please use the 'numberDecimalSeparator' property instead. Gets or sets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Region. |
| [setNumberDecimalSeparator(string)](#setNumberDecimalSeparator-string-)| <b>@deprecated.</b> Please use the 'numberDecimalSeparator' property instead. Gets or sets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Region. |
| [getNumberGroupSeparator()](#getNumberGroupSeparator--)| <b>@deprecated.</b> Please use the 'numberGroupSeparator' property instead. Gets or sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the group separator of current Region. |
| [setNumberGroupSeparator(string)](#setNumberGroupSeparator-string-)| <b>@deprecated.</b> Please use the 'numberGroupSeparator' property instead. Gets or sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the group separator of current Region. |
| [getPassword()](#getPassword--)| <b>@deprecated.</b> Please use the 'password' property instead. Represents Workbook file encryption password. |
| [setPassword(string)](#setPassword-string-)| <b>@deprecated.</b> Please use the 'password' property instead. Represents Workbook file encryption password. |
| [getWriteProtection()](#getWriteProtection--)| <b>@deprecated.</b> Please use the 'writeProtection' property instead. Provides access to the workbook write protection options. |
| [isEncrypted()](#isEncrypted--)| <b>@deprecated.</b> Please use the 'isEncrypted' property instead. Gets a value that indicates whether a password is required to open this workbook. |
| [isProtected()](#isProtected--)| <b>@deprecated.</b> Please use the 'isProtected' property instead. Gets a value that indicates whether the structure or window of the Workbook is protected. |
| [isDefaultEncrypted()](#isDefaultEncrypted--)| <b>@deprecated.</b> Please use the 'isDefaultEncrypted' property instead. Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked. |
| [setIsDefaultEncrypted(boolean)](#setIsDefaultEncrypted-boolean-)| <b>@deprecated.</b> Please use the 'isDefaultEncrypted' property instead. Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked. |
| [isMinimized()](#isMinimized--)| <b>@deprecated.</b> Please use the 'isMinimized' property instead. Represents whether the generated spreadsheet will be opened Minimized. |
| [setIsMinimized(boolean)](#setIsMinimized-boolean-)| <b>@deprecated.</b> Please use the 'isMinimized' property instead. Represents whether the generated spreadsheet will be opened Minimized. |
| [isHidden()](#isHidden--)| <b>@deprecated.</b> Please use the 'isHidden' property instead. Indicates whether this workbook is hidden. |
| [setIsHidden(boolean)](#setIsHidden-boolean-)| <b>@deprecated.</b> Please use the 'isHidden' property instead. Indicates whether this workbook is hidden. |
| [getAutoCompressPictures()](#getAutoCompressPictures--)| <b>@deprecated.</b> Please use the 'autoCompressPictures' property instead. Specifies a boolean value that indicates the application automatically compressed pictures in the workbook. |
| [setAutoCompressPictures(boolean)](#setAutoCompressPictures-boolean-)| <b>@deprecated.</b> Please use the 'autoCompressPictures' property instead. Specifies a boolean value that indicates the application automatically compressed pictures in the workbook. |
| [getRemovePersonalInformation()](#getRemovePersonalInformation--)| <b>@deprecated.</b> Please use the 'removePersonalInformation' property instead. True if personal information can be removed from the specified workbook. |
| [setRemovePersonalInformation(boolean)](#setRemovePersonalInformation-boolean-)| <b>@deprecated.</b> Please use the 'removePersonalInformation' property instead. True if personal information can be removed from the specified workbook. |
| [getHidePivotFieldList()](#getHidePivotFieldList--)| <b>@deprecated.</b> Please use the 'hidePivotFieldList' property instead. Gets and sets whether hide the field list for the PivotTable. |
| [setHidePivotFieldList(boolean)](#setHidePivotFieldList-boolean-)| <b>@deprecated.</b> Please use the 'hidePivotFieldList' property instead. Gets and sets whether hide the field list for the PivotTable. |
| [getMaxUniqueItemsPerField()](#getMaxUniqueItemsPerField--)| <b>@deprecated.</b> Please use the 'maxUniqueItemsPerField' property instead. Gets and set the limitation of unique items per field |
| [setMaxUniqueItemsPerField(number)](#setMaxUniqueItemsPerField-number-)| <b>@deprecated.</b> Please use the 'maxUniqueItemsPerField' property instead. Gets and set the limitation of unique items per field |
| [getUpdateLinksType()](#getUpdateLinksType--)| <b>@deprecated.</b> Please use the 'updateLinksType' property instead. Gets and sets how updates external links when the workbook is opened. |
| [setUpdateLinksType(UpdateLinksType)](#setUpdateLinksType-updatelinkstype-)| <b>@deprecated.</b> Please use the 'updateLinksType' property instead. Gets and sets how updates external links when the workbook is opened. |
| [getMaxRow()](#getMaxRow--)| <b>@deprecated.</b> Please use the 'maxRow' property instead. Gets the max row index, zero-based. |
| [getMaxColumn()](#getMaxColumn--)| <b>@deprecated.</b> Please use the 'maxColumn' property instead. Gets the max column index, zero-based. |
| [getSmartTagOptions()](#getSmartTagOptions--)| <b>@deprecated.</b> Please use the 'smartTagOptions' property instead. Gets the options of the smart tag. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--)| <b>@deprecated.</b> Please use the 'defaultStyleSettings' property instead. Gets the settings for default values of style-related properties for this workbook. |
| [getWindowLeft()](#getWindowLeft--)| <b>@deprecated.</b> Please use the 'windowLeft' property instead. The distance from the left edge of the client area to the left edge of the window, in unit of point. |
| [setWindowLeft(number)](#setWindowLeft-number-)| <b>@deprecated.</b> Please use the 'windowLeft' property instead. The distance from the left edge of the client area to the left edge of the window, in unit of point. |
| [getWindowLeftInch()](#getWindowLeftInch--)| <b>@deprecated.</b> Please use the 'windowLeftInch' property instead. The distance from the left edge of the client area to the left edge of the window. In unit of inch. |
| [setWindowLeftInch(number)](#setWindowLeftInch-number-)| <b>@deprecated.</b> Please use the 'windowLeftInch' property instead. The distance from the left edge of the client area to the left edge of the window. In unit of inch. |
| [getWindowLeftCM()](#getWindowLeftCM--)| <b>@deprecated.</b> Please use the 'windowLeftCM' property instead. The distance from the left edge of the client area to the left edge of the window. In unit of centimeter. |
| [setWindowLeftCM(number)](#setWindowLeftCM-number-)| <b>@deprecated.</b> Please use the 'windowLeftCM' property instead. The distance from the left edge of the client area to the left edge of the window. In unit of centimeter. |
| [getWindowTop()](#getWindowTop--)| <b>@deprecated.</b> Please use the 'windowTop' property instead. The distance from the top edge of the client area to the top edge of the window, in unit of point. |
| [setWindowTop(number)](#setWindowTop-number-)| <b>@deprecated.</b> Please use the 'windowTop' property instead. The distance from the top edge of the client area to the top edge of the window, in unit of point. |
| [getWindowTopInch()](#getWindowTopInch--)| <b>@deprecated.</b> Please use the 'windowTopInch' property instead. The distance from the top edge of the client area to the top edge of the window, in unit of inch. |
| [setWindowTopInch(number)](#setWindowTopInch-number-)| <b>@deprecated.</b> Please use the 'windowTopInch' property instead. The distance from the top edge of the client area to the top edge of the window, in unit of inch. |
| [getWindowTopCM()](#getWindowTopCM--)| <b>@deprecated.</b> Please use the 'windowTopCM' property instead. The distance from the top edge of the client area to the top edge of the window, in unit of centimeter. |
| [setWindowTopCM(number)](#setWindowTopCM-number-)| <b>@deprecated.</b> Please use the 'windowTopCM' property instead. The distance from the top edge of the client area to the top edge of the window, in unit of centimeter. |
| [getWindowWidth()](#getWindowWidth--)| <b>@deprecated.</b> Please use the 'windowWidth' property instead. The width of the window, in unit of point. |
| [setWindowWidth(number)](#setWindowWidth-number-)| <b>@deprecated.</b> Please use the 'windowWidth' property instead. The width of the window, in unit of point. |
| [getWindowWidthInch()](#getWindowWidthInch--)| <b>@deprecated.</b> Please use the 'windowWidthInch' property instead. The width of the window, in unit of inch. |
| [setWindowWidthInch(number)](#setWindowWidthInch-number-)| <b>@deprecated.</b> Please use the 'windowWidthInch' property instead. The width of the window, in unit of inch. |
| [getWindowWidthCM()](#getWindowWidthCM--)| <b>@deprecated.</b> Please use the 'windowWidthCM' property instead. The width of the window, in unit of centimeter. |
| [setWindowWidthCM(number)](#setWindowWidthCM-number-)| <b>@deprecated.</b> Please use the 'windowWidthCM' property instead. The width of the window, in unit of centimeter. |
| [getWindowHeight()](#getWindowHeight--)| <b>@deprecated.</b> Please use the 'windowHeight' property instead. The height of the window, in unit of point. |
| [setWindowHeight(number)](#setWindowHeight-number-)| <b>@deprecated.</b> Please use the 'windowHeight' property instead. The height of the window, in unit of point. |
| [getWindowHeightInch()](#getWindowHeightInch--)| <b>@deprecated.</b> Please use the 'windowHeightInch' property instead. The height of the window, in unit of inch. |
| [setWindowHeightInch(number)](#setWindowHeightInch-number-)| <b>@deprecated.</b> Please use the 'windowHeightInch' property instead. The height of the window, in unit of inch. |
| [getWindowHeightCM()](#getWindowHeightCM--)| <b>@deprecated.</b> Please use the 'windowHeightCM' property instead. The height of the window, in unit of centimeter. |
| [setWindowHeightCM(number)](#setWindowHeightCM-number-)| <b>@deprecated.</b> Please use the 'windowHeightCM' property instead. The height of the window, in unit of centimeter. |
| [getUpdateAdjacentCellsBorder()](#getUpdateAdjacentCellsBorder--)| <b>@deprecated.</b> Please use the 'updateAdjacentCellsBorder' property instead. Indicates whether update adjacent cells' border. |
| [setUpdateAdjacentCellsBorder(boolean)](#setUpdateAdjacentCellsBorder-boolean-)| <b>@deprecated.</b> Please use the 'updateAdjacentCellsBorder' property instead. Indicates whether update adjacent cells' border. |
| [getSignificantDigitsType()](#getSignificantDigitsType--)| <b>@deprecated.</b> Please use the 'significantDigitsType' property instead. Gets and sets the type of significant digits for outputing numeric values in this workbook. Default value is [CellsHelper.SignificantDigitsType](../cellshelper.significantdigitstype/). |
| [setSignificantDigitsType(SignificantDigitsType)](#setSignificantDigitsType-significantdigitstype-)| <b>@deprecated.</b> Please use the 'significantDigitsType' property instead. Gets and sets the type of significant digits for outputing numeric values in this workbook. Default value is [CellsHelper.SignificantDigitsType](../cellshelper.significantdigitstype/). |
| [getCheckCompatibility()](#getCheckCompatibility--)| <b>@deprecated.</b> Please use the 'checkCompatibility' property instead. Indicates whether check compatibility with earlier versions when saving workbook. |
| [setCheckCompatibility(boolean)](#setCheckCompatibility-boolean-)| <b>@deprecated.</b> Please use the 'checkCompatibility' property instead. Indicates whether check compatibility with earlier versions when saving workbook. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--)| <b>@deprecated.</b> Please use the 'checkExcelRestriction' property instead. Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [setCheckExcelRestriction(boolean)](#setCheckExcelRestriction-boolean-)| <b>@deprecated.</b> Please use the 'checkExcelRestriction' property instead. Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [getAutoRecover()](#getAutoRecover--)| <b>@deprecated.</b> Please use the 'autoRecover' property instead. Indicates whether the file is marked for auto-recovery. |
| [setAutoRecover(boolean)](#setAutoRecover-boolean-)| <b>@deprecated.</b> Please use the 'autoRecover' property instead. Indicates whether the file is marked for auto-recovery. |
| [getCrashSave()](#getCrashSave--)| <b>@deprecated.</b> Please use the 'crashSave' property instead. indicates whether the application last saved the workbook file after a crash. |
| [setCrashSave(boolean)](#setCrashSave-boolean-)| <b>@deprecated.</b> Please use the 'crashSave' property instead. indicates whether the application last saved the workbook file after a crash. |
| [getDataExtractLoad()](#getDataExtractLoad--)| <b>@deprecated.</b> Please use the 'dataExtractLoad' property instead. indicates whether the application last opened the workbook for data recovery. |
| [setDataExtractLoad(boolean)](#setDataExtractLoad-boolean-)| <b>@deprecated.</b> Please use the 'dataExtractLoad' property instead. indicates whether the application last opened the workbook for data recovery. |
| [getRepairLoad()](#getRepairLoad--)| <b>@deprecated.</b> Please use the 'repairLoad' property instead. Indicates whether the application last opened the workbook in safe or repair mode. |
| [setRepairLoad(boolean)](#setRepairLoad-boolean-)| <b>@deprecated.</b> Please use the 'repairLoad' property instead. Indicates whether the application last opened the workbook in safe or repair mode. |
| [getBuildVersion()](#getBuildVersion--)| <b>@deprecated.</b> Please use the 'buildVersion' property instead. Specifies the incremental public release of the application. |
| [setBuildVersion(string)](#setBuildVersion-string-)| <b>@deprecated.</b> Please use the 'buildVersion' property instead. Specifies the incremental public release of the application. |
| [getMemorySetting()](#getMemorySetting--)| <b>@deprecated.</b> Please use the 'memorySetting' property instead. Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets. |
| [setMemorySetting(MemorySetting)](#setMemorySetting-memorysetting-)| <b>@deprecated.</b> Please use the 'memorySetting' property instead. Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets. |
| [getPaperSize()](#getPaperSize--)| <b>@deprecated.</b> Please use the 'paperSize' property instead. Gets and sets the default print paper size. |
| [setPaperSize(PaperSizeType)](#setPaperSize-papersizetype-)| <b>@deprecated.</b> Please use the 'paperSize' property instead. Gets and sets the default print paper size. |
| [setWarningCallback(IWarningCallback)](#setWarningCallback-iwarningcallback-)| <b>@deprecated.</b> Please use the 'warningCallback' property instead. Gets or sets warning callback. |
| [getWarningCallback()](#getWarningCallback--)| <b>@deprecated.</b> Please use the 'warningCallback' property instead. Gets or sets warning callback. |
| [getMaxRowsOfSharedFormula()](#getMaxRowsOfSharedFormula--)| <b>@deprecated.</b> Please use the 'maxRowsOfSharedFormula' property instead. Gets and sets the max row number of shared formula. |
| [setMaxRowsOfSharedFormula(number)](#setMaxRowsOfSharedFormula-number-)| <b>@deprecated.</b> Please use the 'maxRowsOfSharedFormula' property instead. Gets and sets the max row number of shared formula. |
| [getCompliance()](#getCompliance--)| <b>@deprecated.</b> Please use the 'compliance' property instead. Specifies the OOXML version for the output document. The default value is Ecma376_2006. |
| [setCompliance(OoxmlCompliance)](#setCompliance-ooxmlcompliance-)| <b>@deprecated.</b> Please use the 'compliance' property instead. Specifies the OOXML version for the output document. The default value is Ecma376_2006. |
| [getQuotePrefixToStyle()](#getQuotePrefixToStyle--)| <b>@deprecated.</b> Please use the 'quotePrefixToStyle' property instead. Indicates whether setting [Style.QuotePrefix](../style.quoteprefix/) property when entering the string value(which starts  with single quote mark ) to the cell |
| [setQuotePrefixToStyle(boolean)](#setQuotePrefixToStyle-boolean-)| <b>@deprecated.</b> Please use the 'quotePrefixToStyle' property instead. Indicates whether setting [Style.QuotePrefix](../style.quoteprefix/) property when entering the string value(which starts  with single quote mark ) to the cell |
| [getFormulaSettings()](#getFormulaSettings--)| <b>@deprecated.</b> Please use the 'formulaSettings' property instead. Gets the settings for formula-related features. |
| [getPropertiesFollowChartPoint()](#getPropertiesFollowChartPoint--)| <b>@deprecated.</b> Please use the 'propertiesFollowChartPoint' property instead. Indicates whether datapoint properties and datalabels in all charts in this workbook follow their reference. |
| [setPropertiesFollowChartPoint(boolean)](#setPropertiesFollowChartPoint-boolean-)| <b>@deprecated.</b> Please use the 'propertiesFollowChartPoint' property instead. Indicates whether datapoint properties and datalabels in all charts in this workbook follow their reference. |
| [getDiscardImageEditData()](#getDiscardImageEditData--)| <b>@deprecated.</b> Please use the 'discardImageEditData' property instead. Indicates whether discarding editting image data. |
| [setDiscardImageEditData(boolean)](#setDiscardImageEditData-boolean-)| <b>@deprecated.</b> Please use the 'discardImageEditData' property instead. Indicates whether discarding editting image data. |
| [getDefaultImageResolution()](#getDefaultImageResolution--)| <b>@deprecated.</b> Please use the 'defaultImageResolution' property instead. Gets and sets default resolution of image. |
| [setDefaultImageResolution(number)](#setDefaultImageResolution-number-)| <b>@deprecated.</b> Please use the 'defaultImageResolution' property instead. Gets and sets default resolution of image. |
| [getWpsCompatibility()](#getWpsCompatibility--)| <b>@deprecated.</b> Please use the 'wpsCompatibility' property instead. Indicates whether to be compatible with WPS. |
| [setWpsCompatibility(boolean)](#setWpsCompatibility-boolean-)| <b>@deprecated.</b> Please use the 'wpsCompatibility' property instead. Indicates whether to be compatible with WPS. |
| [dispose()](#dispose--)| Releases resources. |
| [getThemeFont(FontSchemeType)](#getThemeFont-fontschemetype-)| Gets the default theme font name. |
| [setPageOrientationType(PageOrientationType)](#setPageOrientationType-pageorientationtype-)| Set the type of  print orientation for the whole workbook. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### author {#author--}

Gets and sets the author of the file.

```javascript
author : string;
```


**Remarks**

It''s not set, check  [BuiltInDocumentPropertyCollection.Author](../builtindocumentpropertycollection.author/) first, then check the user of Environment.

### checkCustomNumberFormat {#checkCustomNumberFormat--}

Indicates whether checking custom number format when setting Style.Custom.

```javascript
checkCustomNumberFormat : boolean;
```


### enableMacros {#enableMacros--}

Enable macros;

```javascript
enableMacros : boolean;
```


**Remarks**

Now it only works when copying a worksheet to other worksheet in a workbook.

### date1904 {#date1904--}

Gets or sets a value which represents if the workbook uses the 1904 date system.

```javascript
date1904 : boolean;
```


### protectionType {#protectionType--}

Readonly. Gets the protection type of the workbook.

```javascript
protectionType : ProtectionType;
```


### displayDrawingObjects {#displayDrawingObjects--}

Indicates whether and how to show objects in the workbook.

```javascript
displayDrawingObjects : DisplayDrawingObjects;
```


### sheetTabBarWidth {#sheetTabBarWidth--}

Width of worksheet tab bar (in 1/1000 of window width).

```javascript
sheetTabBarWidth : number;
```


### showTabs {#showTabs--}

Get or sets a value whether the Workbook tabs are displayed.

```javascript
showTabs : boolean;
```


**Remarks**

The default value is true.

**Example**

The following code hides the Sheet Tabs and Tab Scrolling Buttons for the spreadsheet.

```javascript
const { Workbook } = require("aspose.cells.node");

var workbook = new Workbook();
// Hide the spreadsheet tabs.
workbook.settings.showTabs = false;
```

### firstVisibleTab {#firstVisibleTab--}

Gets or sets the first visible worksheet tab.

```javascript
firstVisibleTab : number;
```


### isHScrollBarVisible {#isHScrollBarVisible--}

Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar.

```javascript
isHScrollBarVisible : boolean;
```


**Remarks**

The default value is true.

**Example**

The following code makes the horizontal scroll bar invisible for the spreadsheet.

```javascript
const { Workbook } = require("aspose.cells.node");

var workbook = new Workbook();
// Hide the horizontal scroll bar of the Excel file.
workbook.settings.isHScrollBarVisible = false;
```

### isVScrollBarVisible {#isVScrollBarVisible--}

Gets or sets a value indicating whether the generated spreadsheet will contain a vertical scroll bar.

```javascript
isVScrollBarVisible : boolean;
```


**Remarks**

The default value is true.

**Example**

The following code makes the vertical scroll bar invisible for the spreadsheet.

```javascript
const { Workbook } = require("aspose.cells.node");

var workbook = new Workbook();
// Hide the vertical scroll bar of the Excel file.
workbook.settings.isVScrollBarVisible = false;
```

### shared {#shared--}

Gets or sets a value that indicates whether the Workbook is shared.

```javascript
shared : boolean;
```


**Remarks**

The default value is false.

### languageCode {#languageCode--}

Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file.

```javascript
languageCode : CountryCode;
```


### region {#region--}

Gets or sets the regional settings for workbook.

```javascript
region : CountryCode;
```


**Remarks**

1. Regional settings used by Aspose.Cells component for a workbook loaded from template file: i). For an XLS file, there are fields defined for regional settings and MS Excel does save regional settings data into the file when saving the XLS file. So, we use the saved region in the template file for the workbook. If you do not want to use the region saved in the XLS file, please reset it to the expected one (such as, CountryCode.Default) after loading the template file. And, we save the user specified value (by this method) into the file too when saving an XLS file. ii). For other file formats, such as, XLSX, XLSB...etc., there is no field defined for regional settings in the file format specification. So, we use the regional settings of application's environment for the workbook. And, the user specified value (by this method) cannot be kept for the generated files with those file formats. 2. For the view effect in MS Excel: The applied regional settings here can take effect only at runtime with Aspose.Cells component and not when viewing the generated file with MS Excel. Even for the generated XLS file in which the specified regional settings data has been saved, when viewing/editing it with MS Excel, the used region to perform formatting by MS Excel is always the default regional settings of the environment where MS Excel is running, not the one saved in the file. It is MS Excel's behavior and cannot be changed by code.

### globalizationSettings {#globalizationSettings--}

Gets and sets the globalization settings.

```javascript
globalizationSettings : GlobalizationSettings;
```


### numberDecimalSeparator {#numberDecimalSeparator--}

Gets or sets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Region.

```javascript
numberDecimalSeparator : string;
```


### numberGroupSeparator {#numberGroupSeparator--}

Gets or sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the group separator of current Region.

```javascript
numberGroupSeparator : string;
```


### password {#password--}

Represents Workbook file encryption password.

```javascript
password : string;
```


### writeProtection {#writeProtection--}

Readonly. Provides access to the workbook write protection options.

```javascript
writeProtection : WriteProtection;
```


### isEncrypted {#isEncrypted--}

Readonly. Gets a value that indicates whether a password is required to open this workbook.

```javascript
isEncrypted : boolean;
```


### isProtected {#isProtected--}

Readonly. Gets a value that indicates whether the structure or window of the Workbook is protected.

```javascript
isProtected : boolean;
```


### isDefaultEncrypted {#isDefaultEncrypted--}

Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked.

```javascript
isDefaultEncrypted : boolean;
```


**Remarks**

The default value is false now. It's same as MS Excel 2013.

### isMinimized {#isMinimized--}

Represents whether the generated spreadsheet will be opened Minimized.

```javascript
isMinimized : boolean;
```


### isHidden {#isHidden--}

Indicates whether this workbook is hidden.

```javascript
isHidden : boolean;
```


### autoCompressPictures {#autoCompressPictures--}

Specifies a boolean value that indicates the application automatically compressed pictures in the workbook.

```javascript
autoCompressPictures : boolean;
```


### removePersonalInformation {#removePersonalInformation--}

True if personal information can be removed from the specified workbook.

```javascript
removePersonalInformation : boolean;
```


### hidePivotFieldList {#hidePivotFieldList--}

Gets and sets whether hide the field list for the PivotTable.

```javascript
hidePivotFieldList : boolean;
```


### maxUniqueItemsPerField {#maxUniqueItemsPerField--}

Gets and set the limitation of unique items per field

```javascript
maxUniqueItemsPerField : number;
```


### updateLinksType {#updateLinksType--}

Gets and sets how updates external links when the workbook is opened.

```javascript
updateLinksType : UpdateLinksType;
```


### maxRow {#maxRow--}

Readonly. Gets the max row index, zero-based.

```javascript
maxRow : number;
```


**Remarks**

Returns 65535 if the file format is Excel97-2003;

### maxColumn {#maxColumn--}

Readonly. Gets the max column index, zero-based.

```javascript
maxColumn : number;
```


**Remarks**

Returns 255 if the file format is Excel97-2003;

### smartTagOptions {#smartTagOptions--}

Readonly. Gets the options of the smart tag.

```javascript
smartTagOptions : SmartTagOptions;
```


### defaultStyleSettings {#defaultStyleSettings--}

Readonly. Gets the settings for default values of style-related properties for this workbook.

```javascript
defaultStyleSettings : DefaultStyleSettings;
```


### windowLeft {#windowLeft--}

The distance from the left edge of the client area to the left edge of the window, in unit of point.

```javascript
windowLeft : number;
```


### windowLeftInch {#windowLeftInch--}

The distance from the left edge of the client area to the left edge of the window. In unit of inch.

```javascript
windowLeftInch : number;
```


### windowLeftCM {#windowLeftCM--}

The distance from the left edge of the client area to the left edge of the window. In unit of centimeter.

```javascript
windowLeftCM : number;
```


### windowTop {#windowTop--}

The distance from the top edge of the client area to the top edge of the window, in unit of point.

```javascript
windowTop : number;
```


### windowTopInch {#windowTopInch--}

The distance from the top edge of the client area to the top edge of the window, in unit of inch.

```javascript
windowTopInch : number;
```


### windowTopCM {#windowTopCM--}

The distance from the top edge of the client area to the top edge of the window, in unit of centimeter.

```javascript
windowTopCM : number;
```


### windowWidth {#windowWidth--}

The width of the window, in unit of point.

```javascript
windowWidth : number;
```


### windowWidthInch {#windowWidthInch--}

The width of the window, in unit of inch.

```javascript
windowWidthInch : number;
```


### windowWidthCM {#windowWidthCM--}

The width of the window, in unit of centimeter.

```javascript
windowWidthCM : number;
```


### windowHeight {#windowHeight--}

The height of the window, in unit of point.

```javascript
windowHeight : number;
```


### windowHeightInch {#windowHeightInch--}

The height of the window, in unit of inch.

```javascript
windowHeightInch : number;
```


### windowHeightCM {#windowHeightCM--}

The height of the window, in unit of centimeter.

```javascript
windowHeightCM : number;
```


### updateAdjacentCellsBorder {#updateAdjacentCellsBorder--}

Indicates whether update adjacent cells' border.

```javascript
updateAdjacentCellsBorder : boolean;
```


**Remarks**

The default value is false. For example: the bottom border of the cell A1 is update, the top border of the cell A2 should be changed too.

### significantDigitsType {#significantDigitsType--}

Gets and sets the type of significant digits for outputing numeric values in this workbook. Default value is [CellsHelper.SignificantDigitsType](../cellshelper.significantdigitstype/).

```javascript
significantDigitsType : SignificantDigitsType;
```


### checkCompatibility {#checkCompatibility--}

Indicates whether check compatibility with earlier versions when saving workbook.

```javascript
checkCompatibility : boolean;
```


**Remarks**

The default value is true. Only for Excel97-2003 xls or xlt files.

### checkExcelRestriction {#checkExcelRestriction--}

Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.

```javascript
checkExcelRestriction : boolean;
```


### autoRecover {#autoRecover--}

Indicates whether the file is marked for auto-recovery.

```javascript
autoRecover : boolean;
```


### crashSave {#crashSave--}

indicates whether the application last saved the workbook file after a crash.

```javascript
crashSave : boolean;
```


### dataExtractLoad {#dataExtractLoad--}

indicates whether the application last opened the workbook for data recovery.

```javascript
dataExtractLoad : boolean;
```


### repairLoad {#repairLoad--}

Indicates whether the application last opened the workbook in safe or repair mode.

```javascript
repairLoad : boolean;
```


### buildVersion {#buildVersion--}

Specifies the incremental public release of the application.

```javascript
buildVersion : string;
```


### memorySetting {#memorySetting--}

Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets.

```javascript
memorySetting : MemorySetting;
```


**Remarks**

For more details about memory mode, please see [Cells.MemorySetting](../cells.memorysetting/).

### paperSize {#paperSize--}

Gets and sets the default print paper size.

```javascript
paperSize : PaperSizeType;
```


**Remarks**

If there is no setting about paper size,MS Excel will use default printer's setting.

### warningCallback {#warningCallback--}

Gets or sets warning callback.

```javascript
warningCallback : IWarningCallback;
```


### maxRowsOfSharedFormula {#maxRowsOfSharedFormula--}

Gets and sets the max row number of shared formula.

```javascript
maxRowsOfSharedFormula : number;
```


**Remarks**

If the number is too large, the autofilter works very slow in MS Excel 2013.

### compliance {#compliance--}

Specifies the OOXML version for the output document. The default value is Ecma376_2006.

```javascript
compliance : OoxmlCompliance;
```


**Remarks**

Only for .xlsx files.

### quotePrefixToStyle {#quotePrefixToStyle--}

Indicates whether setting [Style.QuotePrefix](../style.quoteprefix/) property when entering the string value(which starts  with single quote mark ) to the cell

```javascript
quotePrefixToStyle : boolean;
```


### formulaSettings {#formulaSettings--}

Readonly. Gets the settings for formula-related features.

```javascript
formulaSettings : FormulaSettings;
```


### propertiesFollowChartPoint {#propertiesFollowChartPoint--}

Indicates whether datapoint properties and datalabels in all charts in this workbook follow their reference.

```javascript
propertiesFollowChartPoint : boolean;
```


### discardImageEditData {#discardImageEditData--}

Indicates whether discarding editting image data.

```javascript
discardImageEditData : boolean;
```


### defaultImageResolution {#defaultImageResolution--}

Gets and sets default resolution of image.

```javascript
defaultImageResolution : number;
```


### wpsCompatibility {#wpsCompatibility--}

Indicates whether to be compatible with WPS.

```javascript
wpsCompatibility : boolean;
```


### getAuthor() {#getAuthor--}

<b>@deprecated.</b> Please use the 'author' property instead. Gets and sets the author of the file.

```javascript
getAuthor() : string;
```


**Remarks**

It''s not set, check  [BuiltInDocumentPropertyCollection.Author](../builtindocumentpropertycollection.author/) first, then check the user of Environment.

### setAuthor(string) {#setAuthor-string-}

<b>@deprecated.</b> Please use the 'author' property instead. Gets and sets the author of the file.

```javascript
setAuthor(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

It''s not set, check  [BuiltInDocumentPropertyCollection.Author](../builtindocumentpropertycollection.author/) first, then check the user of Environment.

### getCheckCustomNumberFormat() {#getCheckCustomNumberFormat--}

<b>@deprecated.</b> Please use the 'checkCustomNumberFormat' property instead. Indicates whether checking custom number format when setting Style.Custom.

```javascript
getCheckCustomNumberFormat() : boolean;
```


### setCheckCustomNumberFormat(boolean) {#setCheckCustomNumberFormat-boolean-}

<b>@deprecated.</b> Please use the 'checkCustomNumberFormat' property instead. Indicates whether checking custom number format when setting Style.Custom.

```javascript
setCheckCustomNumberFormat(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getEnableMacros() {#getEnableMacros--}

<b>@deprecated.</b> Please use the 'enableMacros' property instead. Enable macros;

```javascript
getEnableMacros() : boolean;
```


**Remarks**

Now it only works when copying a worksheet to other worksheet in a workbook.

### setEnableMacros(boolean) {#setEnableMacros-boolean-}

<b>@deprecated.</b> Please use the 'enableMacros' property instead. Enable macros;

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

<b>@deprecated.</b> Please use the 'date1904' property instead. Gets or sets a value which represents if the workbook uses the 1904 date system.

```javascript
getDate1904() : boolean;
```


### setDate1904(boolean) {#setDate1904-boolean-}

<b>@deprecated.</b> Please use the 'date1904' property instead. Gets or sets a value which represents if the workbook uses the 1904 date system.

```javascript
setDate1904(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getProtectionType() {#getProtectionType--}

<b>@deprecated.</b> Please use the 'protectionType' property instead. Gets the protection type of the workbook.

```javascript
getProtectionType() : ProtectionType;
```


**Returns**

[ProtectionType](../protectiontype/)

### getDisplayDrawingObjects() {#getDisplayDrawingObjects--}

<b>@deprecated.</b> Please use the 'displayDrawingObjects' property instead. Indicates whether and how to show objects in the workbook.

```javascript
getDisplayDrawingObjects() : DisplayDrawingObjects;
```


**Returns**

[DisplayDrawingObjects](../displaydrawingobjects/)

### setDisplayDrawingObjects(DisplayDrawingObjects) {#setDisplayDrawingObjects-displaydrawingobjects-}

<b>@deprecated.</b> Please use the 'displayDrawingObjects' property instead. Indicates whether and how to show objects in the workbook.

```javascript
setDisplayDrawingObjects(value: DisplayDrawingObjects) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DisplayDrawingObjects](../displaydrawingobjects/) | The value to set. |

### getSheetTabBarWidth() {#getSheetTabBarWidth--}

<b>@deprecated.</b> Please use the 'sheetTabBarWidth' property instead. Width of worksheet tab bar (in 1/1000 of window width).

```javascript
getSheetTabBarWidth() : number;
```


### setSheetTabBarWidth(number) {#setSheetTabBarWidth-number-}

<b>@deprecated.</b> Please use the 'sheetTabBarWidth' property instead. Width of worksheet tab bar (in 1/1000 of window width).

```javascript
setSheetTabBarWidth(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getShowTabs() {#getShowTabs--}

<b>@deprecated.</b> Please use the 'showTabs' property instead. Get or sets a value whether the Workbook tabs are displayed.

```javascript
getShowTabs() : boolean;
```


**Remarks**

The default value is true.

### setShowTabs(boolean) {#setShowTabs-boolean-}

<b>@deprecated.</b> Please use the 'showTabs' property instead. Get or sets a value whether the Workbook tabs are displayed.

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

<b>@deprecated.</b> Please use the 'firstVisibleTab' property instead. Gets or sets the first visible worksheet tab.

```javascript
getFirstVisibleTab() : number;
```


### setFirstVisibleTab(number) {#setFirstVisibleTab-number-}

<b>@deprecated.</b> Please use the 'firstVisibleTab' property instead. Gets or sets the first visible worksheet tab.

```javascript
setFirstVisibleTab(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### isHScrollBarVisible() {#isHScrollBarVisible--}

<b>@deprecated.</b> Please use the 'isHScrollBarVisible' property instead. Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar.

```javascript
isHScrollBarVisible() : boolean;
```


**Remarks**

The default value is true.

### setIsHScrollBarVisible(boolean) {#setIsHScrollBarVisible-boolean-}

<b>@deprecated.</b> Please use the 'isHScrollBarVisible' property instead. Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar.

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

<b>@deprecated.</b> Please use the 'isVScrollBarVisible' property instead. Gets or sets a value indicating whether the generated spreadsheet will contain a vertical scroll bar.

```javascript
isVScrollBarVisible() : boolean;
```


**Remarks**

The default value is true.

### setIsVScrollBarVisible(boolean) {#setIsVScrollBarVisible-boolean-}

<b>@deprecated.</b> Please use the 'isVScrollBarVisible' property instead. Gets or sets a value indicating whether the generated spreadsheet will contain a vertical scroll bar.

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

<b>@deprecated.</b> Please use the 'shared' property instead. Gets or sets a value that indicates whether the Workbook is shared.

```javascript
getShared() : boolean;
```


**Remarks**

The default value is false.

### setShared(boolean) {#setShared-boolean-}

<b>@deprecated.</b> Please use the 'shared' property instead. Gets or sets a value that indicates whether the Workbook is shared.

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

<b>@deprecated.</b> Please use the 'languageCode' property instead. Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file.

```javascript
getLanguageCode() : CountryCode;
```


**Returns**

[CountryCode](../countrycode/)

### setLanguageCode(CountryCode) {#setLanguageCode-countrycode-}

<b>@deprecated.</b> Please use the 'languageCode' property instead. Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file.

```javascript
setLanguageCode(value: CountryCode) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CountryCode](../countrycode/) | The value to set. |

### getRegion() {#getRegion--}

<b>@deprecated.</b> Please use the 'region' property instead. Gets or sets the regional settings for workbook.

```javascript
getRegion() : CountryCode;
```


**Returns**

[CountryCode](../countrycode/)

**Remarks**

1. Regional settings used by Aspose.Cells component for a workbook loaded from template file: i). For an XLS file, there are fields defined for regional settings and MS Excel does save regional settings data into the file when saving the XLS file. So, we use the saved region in the template file for the workbook. If you do not want to use the region saved in the XLS file, please reset it to the expected one (such as, CountryCode.Default) after loading the template file. And, we save the user specified value (by this method) into the file too when saving an XLS file. ii). For other file formats, such as, XLSX, XLSB...etc., there is no field defined for regional settings in the file format specification. So, we use the regional settings of application's environment for the workbook. And, the user specified value (by this method) cannot be kept for the generated files with those file formats. 2. For the view effect in MS Excel: The applied regional settings here can take effect only at runtime with Aspose.Cells component and not when viewing the generated file with MS Excel. Even for the generated XLS file in which the specified regional settings data has been saved, when viewing/editing it with MS Excel, the used region to perform formatting by MS Excel is always the default regional settings of the environment where MS Excel is running, not the one saved in the file. It is MS Excel's behavior and cannot be changed by code.

### setRegion(CountryCode) {#setRegion-countrycode-}

<b>@deprecated.</b> Please use the 'region' property instead. Gets or sets the regional settings for workbook.

```javascript
setRegion(value: CountryCode) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CountryCode](../countrycode/) | The value to set. |

**Remarks**

1. Regional settings used by Aspose.Cells component for a workbook loaded from template file: i). For an XLS file, there are fields defined for regional settings and MS Excel does save regional settings data into the file when saving the XLS file. So, we use the saved region in the template file for the workbook. If you do not want to use the region saved in the XLS file, please reset it to the expected one (such as, CountryCode.Default) after loading the template file. And, we save the user specified value (by this method) into the file too when saving an XLS file. ii). For other file formats, such as, XLSX, XLSB...etc., there is no field defined for regional settings in the file format specification. So, we use the regional settings of application's environment for the workbook. And, the user specified value (by this method) cannot be kept for the generated files with those file formats. 2. For the view effect in MS Excel: The applied regional settings here can take effect only at runtime with Aspose.Cells component and not when viewing the generated file with MS Excel. Even for the generated XLS file in which the specified regional settings data has been saved, when viewing/editing it with MS Excel, the used region to perform formatting by MS Excel is always the default regional settings of the environment where MS Excel is running, not the one saved in the file. It is MS Excel's behavior and cannot be changed by code.

### getGlobalizationSettings() {#getGlobalizationSettings--}

<b>@deprecated.</b> Please use the 'globalizationSettings' property instead. Gets and sets the globalization settings.

```javascript
getGlobalizationSettings() : GlobalizationSettings;
```


**Returns**

[GlobalizationSettings](../globalizationsettings/)

### setGlobalizationSettings(GlobalizationSettings) {#setGlobalizationSettings-globalizationsettings-}

<b>@deprecated.</b> Please use the 'globalizationSettings' property instead. Gets and sets the globalization settings.

```javascript
setGlobalizationSettings(value: GlobalizationSettings) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GlobalizationSettings](../globalizationsettings/) | The value to set. |

### getNumberDecimalSeparator() {#getNumberDecimalSeparator--}

<b>@deprecated.</b> Please use the 'numberDecimalSeparator' property instead. Gets or sets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Region.

```javascript
getNumberDecimalSeparator() : string;
```


### setNumberDecimalSeparator(string) {#setNumberDecimalSeparator-string-}

<b>@deprecated.</b> Please use the 'numberDecimalSeparator' property instead. Gets or sets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Region.

```javascript
setNumberDecimalSeparator(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getNumberGroupSeparator() {#getNumberGroupSeparator--}

<b>@deprecated.</b> Please use the 'numberGroupSeparator' property instead. Gets or sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the group separator of current Region.

```javascript
getNumberGroupSeparator() : string;
```


### setNumberGroupSeparator(string) {#setNumberGroupSeparator-string-}

<b>@deprecated.</b> Please use the 'numberGroupSeparator' property instead. Gets or sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the group separator of current Region.

```javascript
setNumberGroupSeparator(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getPassword() {#getPassword--}

<b>@deprecated.</b> Please use the 'password' property instead. Represents Workbook file encryption password.

```javascript
getPassword() : string;
```


### setPassword(string) {#setPassword-string-}

<b>@deprecated.</b> Please use the 'password' property instead. Represents Workbook file encryption password.

```javascript
setPassword(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getWriteProtection() {#getWriteProtection--}

<b>@deprecated.</b> Please use the 'writeProtection' property instead. Provides access to the workbook write protection options.

```javascript
getWriteProtection() : WriteProtection;
```


**Returns**

[WriteProtection](../writeprotection/)

### isEncrypted() {#isEncrypted--}

<b>@deprecated.</b> Please use the 'isEncrypted' property instead. Gets a value that indicates whether a password is required to open this workbook.

```javascript
isEncrypted() : boolean;
```


### isProtected() {#isProtected--}

<b>@deprecated.</b> Please use the 'isProtected' property instead. Gets a value that indicates whether the structure or window of the Workbook is protected.

```javascript
isProtected() : boolean;
```


### isDefaultEncrypted() {#isDefaultEncrypted--}

<b>@deprecated.</b> Please use the 'isDefaultEncrypted' property instead. Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked.

```javascript
isDefaultEncrypted() : boolean;
```


**Remarks**

The default value is false now. It's same as MS Excel 2013.

### setIsDefaultEncrypted(boolean) {#setIsDefaultEncrypted-boolean-}

<b>@deprecated.</b> Please use the 'isDefaultEncrypted' property instead. Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked.

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

<b>@deprecated.</b> Please use the 'isMinimized' property instead. Represents whether the generated spreadsheet will be opened Minimized.

```javascript
isMinimized() : boolean;
```


### setIsMinimized(boolean) {#setIsMinimized-boolean-}

<b>@deprecated.</b> Please use the 'isMinimized' property instead. Represents whether the generated spreadsheet will be opened Minimized.

```javascript
setIsMinimized(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isHidden() {#isHidden--}

<b>@deprecated.</b> Please use the 'isHidden' property instead. Indicates whether this workbook is hidden.

```javascript
isHidden() : boolean;
```


### setIsHidden(boolean) {#setIsHidden-boolean-}

<b>@deprecated.</b> Please use the 'isHidden' property instead. Indicates whether this workbook is hidden.

```javascript
setIsHidden(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAutoCompressPictures() {#getAutoCompressPictures--}

<b>@deprecated.</b> Please use the 'autoCompressPictures' property instead. Specifies a boolean value that indicates the application automatically compressed pictures in the workbook.

```javascript
getAutoCompressPictures() : boolean;
```


### setAutoCompressPictures(boolean) {#setAutoCompressPictures-boolean-}

<b>@deprecated.</b> Please use the 'autoCompressPictures' property instead. Specifies a boolean value that indicates the application automatically compressed pictures in the workbook.

```javascript
setAutoCompressPictures(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getRemovePersonalInformation() {#getRemovePersonalInformation--}

<b>@deprecated.</b> Please use the 'removePersonalInformation' property instead. True if personal information can be removed from the specified workbook.

```javascript
getRemovePersonalInformation() : boolean;
```


### setRemovePersonalInformation(boolean) {#setRemovePersonalInformation-boolean-}

<b>@deprecated.</b> Please use the 'removePersonalInformation' property instead. True if personal information can be removed from the specified workbook.

```javascript
setRemovePersonalInformation(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getHidePivotFieldList() {#getHidePivotFieldList--}

<b>@deprecated.</b> Please use the 'hidePivotFieldList' property instead. Gets and sets whether hide the field list for the PivotTable.

```javascript
getHidePivotFieldList() : boolean;
```


### setHidePivotFieldList(boolean) {#setHidePivotFieldList-boolean-}

<b>@deprecated.</b> Please use the 'hidePivotFieldList' property instead. Gets and sets whether hide the field list for the PivotTable.

```javascript
setHidePivotFieldList(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getMaxUniqueItemsPerField() {#getMaxUniqueItemsPerField--}

<b>@deprecated.</b> Please use the 'maxUniqueItemsPerField' property instead. Gets and set the limitation of unique items per field

```javascript
getMaxUniqueItemsPerField() : number;
```


### setMaxUniqueItemsPerField(number) {#setMaxUniqueItemsPerField-number-}

<b>@deprecated.</b> Please use the 'maxUniqueItemsPerField' property instead. Gets and set the limitation of unique items per field

```javascript
setMaxUniqueItemsPerField(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getUpdateLinksType() {#getUpdateLinksType--}

<b>@deprecated.</b> Please use the 'updateLinksType' property instead. Gets and sets how updates external links when the workbook is opened.

```javascript
getUpdateLinksType() : UpdateLinksType;
```


**Returns**

[UpdateLinksType](../updatelinkstype/)

### setUpdateLinksType(UpdateLinksType) {#setUpdateLinksType-updatelinkstype-}

<b>@deprecated.</b> Please use the 'updateLinksType' property instead. Gets and sets how updates external links when the workbook is opened.

```javascript
setUpdateLinksType(value: UpdateLinksType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [UpdateLinksType](../updatelinkstype/) | The value to set. |

### getMaxRow() {#getMaxRow--}

<b>@deprecated.</b> Please use the 'maxRow' property instead. Gets the max row index, zero-based.

```javascript
getMaxRow() : number;
```


**Remarks**

Returns 65535 if the file format is Excel97-2003;

### getMaxColumn() {#getMaxColumn--}

<b>@deprecated.</b> Please use the 'maxColumn' property instead. Gets the max column index, zero-based.

```javascript
getMaxColumn() : number;
```


**Remarks**

Returns 255 if the file format is Excel97-2003;

### getSmartTagOptions() {#getSmartTagOptions--}

<b>@deprecated.</b> Please use the 'smartTagOptions' property instead. Gets the options of the smart tag.

```javascript
getSmartTagOptions() : SmartTagOptions;
```


**Returns**

[SmartTagOptions](../smarttagoptions/)

### getDefaultStyleSettings() {#getDefaultStyleSettings--}

<b>@deprecated.</b> Please use the 'defaultStyleSettings' property instead. Gets the settings for default values of style-related properties for this workbook.

```javascript
getDefaultStyleSettings() : DefaultStyleSettings;
```


**Returns**

[DefaultStyleSettings](../defaultstylesettings/)

### getWindowLeft() {#getWindowLeft--}

<b>@deprecated.</b> Please use the 'windowLeft' property instead. The distance from the left edge of the client area to the left edge of the window, in unit of point.

```javascript
getWindowLeft() : number;
```


### setWindowLeft(number) {#setWindowLeft-number-}

<b>@deprecated.</b> Please use the 'windowLeft' property instead. The distance from the left edge of the client area to the left edge of the window, in unit of point.

```javascript
setWindowLeft(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWindowLeftInch() {#getWindowLeftInch--}

<b>@deprecated.</b> Please use the 'windowLeftInch' property instead. The distance from the left edge of the client area to the left edge of the window. In unit of inch.

```javascript
getWindowLeftInch() : number;
```


### setWindowLeftInch(number) {#setWindowLeftInch-number-}

<b>@deprecated.</b> Please use the 'windowLeftInch' property instead. The distance from the left edge of the client area to the left edge of the window. In unit of inch.

```javascript
setWindowLeftInch(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWindowLeftCM() {#getWindowLeftCM--}

<b>@deprecated.</b> Please use the 'windowLeftCM' property instead. The distance from the left edge of the client area to the left edge of the window. In unit of centimeter.

```javascript
getWindowLeftCM() : number;
```


### setWindowLeftCM(number) {#setWindowLeftCM-number-}

<b>@deprecated.</b> Please use the 'windowLeftCM' property instead. The distance from the left edge of the client area to the left edge of the window. In unit of centimeter.

```javascript
setWindowLeftCM(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWindowTop() {#getWindowTop--}

<b>@deprecated.</b> Please use the 'windowTop' property instead. The distance from the top edge of the client area to the top edge of the window, in unit of point.

```javascript
getWindowTop() : number;
```


### setWindowTop(number) {#setWindowTop-number-}

<b>@deprecated.</b> Please use the 'windowTop' property instead. The distance from the top edge of the client area to the top edge of the window, in unit of point.

```javascript
setWindowTop(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWindowTopInch() {#getWindowTopInch--}

<b>@deprecated.</b> Please use the 'windowTopInch' property instead. The distance from the top edge of the client area to the top edge of the window, in unit of inch.

```javascript
getWindowTopInch() : number;
```


### setWindowTopInch(number) {#setWindowTopInch-number-}

<b>@deprecated.</b> Please use the 'windowTopInch' property instead. The distance from the top edge of the client area to the top edge of the window, in unit of inch.

```javascript
setWindowTopInch(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWindowTopCM() {#getWindowTopCM--}

<b>@deprecated.</b> Please use the 'windowTopCM' property instead. The distance from the top edge of the client area to the top edge of the window, in unit of centimeter.

```javascript
getWindowTopCM() : number;
```


### setWindowTopCM(number) {#setWindowTopCM-number-}

<b>@deprecated.</b> Please use the 'windowTopCM' property instead. The distance from the top edge of the client area to the top edge of the window, in unit of centimeter.

```javascript
setWindowTopCM(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWindowWidth() {#getWindowWidth--}

<b>@deprecated.</b> Please use the 'windowWidth' property instead. The width of the window, in unit of point.

```javascript
getWindowWidth() : number;
```


### setWindowWidth(number) {#setWindowWidth-number-}

<b>@deprecated.</b> Please use the 'windowWidth' property instead. The width of the window, in unit of point.

```javascript
setWindowWidth(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWindowWidthInch() {#getWindowWidthInch--}

<b>@deprecated.</b> Please use the 'windowWidthInch' property instead. The width of the window, in unit of inch.

```javascript
getWindowWidthInch() : number;
```


### setWindowWidthInch(number) {#setWindowWidthInch-number-}

<b>@deprecated.</b> Please use the 'windowWidthInch' property instead. The width of the window, in unit of inch.

```javascript
setWindowWidthInch(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWindowWidthCM() {#getWindowWidthCM--}

<b>@deprecated.</b> Please use the 'windowWidthCM' property instead. The width of the window, in unit of centimeter.

```javascript
getWindowWidthCM() : number;
```


### setWindowWidthCM(number) {#setWindowWidthCM-number-}

<b>@deprecated.</b> Please use the 'windowWidthCM' property instead. The width of the window, in unit of centimeter.

```javascript
setWindowWidthCM(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWindowHeight() {#getWindowHeight--}

<b>@deprecated.</b> Please use the 'windowHeight' property instead. The height of the window, in unit of point.

```javascript
getWindowHeight() : number;
```


### setWindowHeight(number) {#setWindowHeight-number-}

<b>@deprecated.</b> Please use the 'windowHeight' property instead. The height of the window, in unit of point.

```javascript
setWindowHeight(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWindowHeightInch() {#getWindowHeightInch--}

<b>@deprecated.</b> Please use the 'windowHeightInch' property instead. The height of the window, in unit of inch.

```javascript
getWindowHeightInch() : number;
```


### setWindowHeightInch(number) {#setWindowHeightInch-number-}

<b>@deprecated.</b> Please use the 'windowHeightInch' property instead. The height of the window, in unit of inch.

```javascript
setWindowHeightInch(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWindowHeightCM() {#getWindowHeightCM--}

<b>@deprecated.</b> Please use the 'windowHeightCM' property instead. The height of the window, in unit of centimeter.

```javascript
getWindowHeightCM() : number;
```


### setWindowHeightCM(number) {#setWindowHeightCM-number-}

<b>@deprecated.</b> Please use the 'windowHeightCM' property instead. The height of the window, in unit of centimeter.

```javascript
setWindowHeightCM(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getUpdateAdjacentCellsBorder() {#getUpdateAdjacentCellsBorder--}

<b>@deprecated.</b> Please use the 'updateAdjacentCellsBorder' property instead. Indicates whether update adjacent cells' border.

```javascript
getUpdateAdjacentCellsBorder() : boolean;
```


**Remarks**

The default value is false. For example: the bottom border of the cell A1 is update, the top border of the cell A2 should be changed too.

### setUpdateAdjacentCellsBorder(boolean) {#setUpdateAdjacentCellsBorder-boolean-}

<b>@deprecated.</b> Please use the 'updateAdjacentCellsBorder' property instead. Indicates whether update adjacent cells' border.

```javascript
setUpdateAdjacentCellsBorder(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is false. For example: the bottom border of the cell A1 is update, the top border of the cell A2 should be changed too.

### getSignificantDigitsType() {#getSignificantDigitsType--}

<b>@deprecated.</b> Please use the 'significantDigitsType' property instead. Gets and sets the type of significant digits for outputing numeric values in this workbook. Default value is [CellsHelper.SignificantDigitsType](../cellshelper.significantdigitstype/).

```javascript
getSignificantDigitsType() : SignificantDigitsType;
```


**Returns**

[SignificantDigitsType](../significantdigitstype/)

### setSignificantDigitsType(SignificantDigitsType) {#setSignificantDigitsType-significantdigitstype-}

<b>@deprecated.</b> Please use the 'significantDigitsType' property instead. Gets and sets the type of significant digits for outputing numeric values in this workbook. Default value is [CellsHelper.SignificantDigitsType](../cellshelper.significantdigitstype/).

```javascript
setSignificantDigitsType(value: SignificantDigitsType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SignificantDigitsType](../significantdigitstype/) | The value to set. |

### getCheckCompatibility() {#getCheckCompatibility--}

<b>@deprecated.</b> Please use the 'checkCompatibility' property instead. Indicates whether check compatibility with earlier versions when saving workbook.

```javascript
getCheckCompatibility() : boolean;
```


**Remarks**

The default value is true. Only for Excel97-2003 xls or xlt files.

### setCheckCompatibility(boolean) {#setCheckCompatibility-boolean-}

<b>@deprecated.</b> Please use the 'checkCompatibility' property instead. Indicates whether check compatibility with earlier versions when saving workbook.

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

<b>@deprecated.</b> Please use the 'checkExcelRestriction' property instead. Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.

```javascript
getCheckExcelRestriction() : boolean;
```


### setCheckExcelRestriction(boolean) {#setCheckExcelRestriction-boolean-}

<b>@deprecated.</b> Please use the 'checkExcelRestriction' property instead. Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.

```javascript
setCheckExcelRestriction(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAutoRecover() {#getAutoRecover--}

<b>@deprecated.</b> Please use the 'autoRecover' property instead. Indicates whether the file is marked for auto-recovery.

```javascript
getAutoRecover() : boolean;
```


### setAutoRecover(boolean) {#setAutoRecover-boolean-}

<b>@deprecated.</b> Please use the 'autoRecover' property instead. Indicates whether the file is marked for auto-recovery.

```javascript
setAutoRecover(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCrashSave() {#getCrashSave--}

<b>@deprecated.</b> Please use the 'crashSave' property instead. indicates whether the application last saved the workbook file after a crash.

```javascript
getCrashSave() : boolean;
```


### setCrashSave(boolean) {#setCrashSave-boolean-}

<b>@deprecated.</b> Please use the 'crashSave' property instead. indicates whether the application last saved the workbook file after a crash.

```javascript
setCrashSave(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getDataExtractLoad() {#getDataExtractLoad--}

<b>@deprecated.</b> Please use the 'dataExtractLoad' property instead. indicates whether the application last opened the workbook for data recovery.

```javascript
getDataExtractLoad() : boolean;
```


### setDataExtractLoad(boolean) {#setDataExtractLoad-boolean-}

<b>@deprecated.</b> Please use the 'dataExtractLoad' property instead. indicates whether the application last opened the workbook for data recovery.

```javascript
setDataExtractLoad(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getRepairLoad() {#getRepairLoad--}

<b>@deprecated.</b> Please use the 'repairLoad' property instead. Indicates whether the application last opened the workbook in safe or repair mode.

```javascript
getRepairLoad() : boolean;
```


### setRepairLoad(boolean) {#setRepairLoad-boolean-}

<b>@deprecated.</b> Please use the 'repairLoad' property instead. Indicates whether the application last opened the workbook in safe or repair mode.

```javascript
setRepairLoad(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getBuildVersion() {#getBuildVersion--}

<b>@deprecated.</b> Please use the 'buildVersion' property instead. Specifies the incremental public release of the application.

```javascript
getBuildVersion() : string;
```


### setBuildVersion(string) {#setBuildVersion-string-}

<b>@deprecated.</b> Please use the 'buildVersion' property instead. Specifies the incremental public release of the application.

```javascript
setBuildVersion(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getMemorySetting() {#getMemorySetting--}

<b>@deprecated.</b> Please use the 'memorySetting' property instead. Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets.

```javascript
getMemorySetting() : MemorySetting;
```


**Returns**

[MemorySetting](../memorysetting/)

**Remarks**

For more details about memory mode, please see [Cells.MemorySetting](../cells.memorysetting/).

### setMemorySetting(MemorySetting) {#setMemorySetting-memorysetting-}

<b>@deprecated.</b> Please use the 'memorySetting' property instead. Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets.

```javascript
setMemorySetting(value: MemorySetting) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MemorySetting](../memorysetting/) | The value to set. |

**Remarks**

For more details about memory mode, please see [Cells.MemorySetting](../cells.memorysetting/).

### getPaperSize() {#getPaperSize--}

<b>@deprecated.</b> Please use the 'paperSize' property instead. Gets and sets the default print paper size.

```javascript
getPaperSize() : PaperSizeType;
```


**Returns**

[PaperSizeType](../papersizetype/)

**Remarks**

If there is no setting about paper size,MS Excel will use default printer's setting.

### setPaperSize(PaperSizeType) {#setPaperSize-papersizetype-}

<b>@deprecated.</b> Please use the 'paperSize' property instead. Gets and sets the default print paper size.

```javascript
setPaperSize(value: PaperSizeType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PaperSizeType](../papersizetype/) | The value to set. |

**Remarks**

If there is no setting about paper size,MS Excel will use default printer's setting.

### setWarningCallback(IWarningCallback) {#setWarningCallback-iwarningcallback-}

<b>@deprecated.</b> Please use the 'warningCallback' property instead. Gets or sets warning callback.

```javascript
setWarningCallback(value: IWarningCallback) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IWarningCallback](../iwarningcallback/) | The value to set. |

### getWarningCallback() {#getWarningCallback--}

<b>@deprecated.</b> Please use the 'warningCallback' property instead. Gets or sets warning callback.

```javascript
getWarningCallback() : IWarningCallback;
```


**Returns**

[IWarningCallback](../iwarningcallback/)

### getMaxRowsOfSharedFormula() {#getMaxRowsOfSharedFormula--}

<b>@deprecated.</b> Please use the 'maxRowsOfSharedFormula' property instead. Gets and sets the max row number of shared formula.

```javascript
getMaxRowsOfSharedFormula() : number;
```


**Remarks**

If the number is too large, the autofilter works very slow in MS Excel 2013.

### setMaxRowsOfSharedFormula(number) {#setMaxRowsOfSharedFormula-number-}

<b>@deprecated.</b> Please use the 'maxRowsOfSharedFormula' property instead. Gets and sets the max row number of shared formula.

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

<b>@deprecated.</b> Please use the 'compliance' property instead. Specifies the OOXML version for the output document. The default value is Ecma376_2006.

```javascript
getCompliance() : OoxmlCompliance;
```


**Returns**

[OoxmlCompliance](../ooxmlcompliance/)

**Remarks**

Only for .xlsx files.

### setCompliance(OoxmlCompliance) {#setCompliance-ooxmlcompliance-}

<b>@deprecated.</b> Please use the 'compliance' property instead. Specifies the OOXML version for the output document. The default value is Ecma376_2006.

```javascript
setCompliance(value: OoxmlCompliance) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [OoxmlCompliance](../ooxmlcompliance/) | The value to set. |

**Remarks**

Only for .xlsx files.

### getQuotePrefixToStyle() {#getQuotePrefixToStyle--}

<b>@deprecated.</b> Please use the 'quotePrefixToStyle' property instead. Indicates whether setting [Style.QuotePrefix](../style.quoteprefix/) property when entering the string value(which starts  with single quote mark ) to the cell

```javascript
getQuotePrefixToStyle() : boolean;
```


### setQuotePrefixToStyle(boolean) {#setQuotePrefixToStyle-boolean-}

<b>@deprecated.</b> Please use the 'quotePrefixToStyle' property instead. Indicates whether setting [Style.QuotePrefix](../style.quoteprefix/) property when entering the string value(which starts  with single quote mark ) to the cell

```javascript
setQuotePrefixToStyle(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getFormulaSettings() {#getFormulaSettings--}

<b>@deprecated.</b> Please use the 'formulaSettings' property instead. Gets the settings for formula-related features.

```javascript
getFormulaSettings() : FormulaSettings;
```


**Returns**

[FormulaSettings](../formulasettings/)

### getPropertiesFollowChartPoint() {#getPropertiesFollowChartPoint--}

<b>@deprecated.</b> Please use the 'propertiesFollowChartPoint' property instead. Indicates whether datapoint properties and datalabels in all charts in this workbook follow their reference.

```javascript
getPropertiesFollowChartPoint() : boolean;
```


### setPropertiesFollowChartPoint(boolean) {#setPropertiesFollowChartPoint-boolean-}

<b>@deprecated.</b> Please use the 'propertiesFollowChartPoint' property instead. Indicates whether datapoint properties and datalabels in all charts in this workbook follow their reference.

```javascript
setPropertiesFollowChartPoint(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getDiscardImageEditData() {#getDiscardImageEditData--}

<b>@deprecated.</b> Please use the 'discardImageEditData' property instead. Indicates whether discarding editting image data.

```javascript
getDiscardImageEditData() : boolean;
```


### setDiscardImageEditData(boolean) {#setDiscardImageEditData-boolean-}

<b>@deprecated.</b> Please use the 'discardImageEditData' property instead. Indicates whether discarding editting image data.

```javascript
setDiscardImageEditData(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getDefaultImageResolution() {#getDefaultImageResolution--}

<b>@deprecated.</b> Please use the 'defaultImageResolution' property instead. Gets and sets default resolution of image.

```javascript
getDefaultImageResolution() : number;
```


### setDefaultImageResolution(number) {#setDefaultImageResolution-number-}

<b>@deprecated.</b> Please use the 'defaultImageResolution' property instead. Gets and sets default resolution of image.

```javascript
setDefaultImageResolution(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWpsCompatibility() {#getWpsCompatibility--}

<b>@deprecated.</b> Please use the 'wpsCompatibility' property instead. Indicates whether to be compatible with WPS.

```javascript
getWpsCompatibility() : boolean;
```


### setWpsCompatibility(boolean) {#setWpsCompatibility-boolean-}

<b>@deprecated.</b> Please use the 'wpsCompatibility' property instead. Indicates whether to be compatible with WPS.

```javascript
setWpsCompatibility(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

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
| type | [FontSchemeType](../fontschemetype/) | The scheme type of the font. |

### setPageOrientationType(PageOrientationType) {#setPageOrientationType-pageorientationtype-}

Set the type of  print orientation for the whole workbook.

```javascript
setPageOrientationType(pageOrientationType: PageOrientationType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageOrientationType | [PageOrientationType](../pageorientationtype/) | The page orientation type |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



