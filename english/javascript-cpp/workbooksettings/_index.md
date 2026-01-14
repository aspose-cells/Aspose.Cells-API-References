---
title: WorkbookSettings
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents all settings of the workbook.
type: docs
url: /javascript-cpp/workbooksettings/
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
| [dispose()](#dispose--)| Releases resources. |
| [getThemeFont(FontSchemeType)](#getThemeFont-fontschemetype-)| Gets the default theme font name. |
| [setPageOrientationType(PageOrientationType)](#setPageOrientationType-pageorientationtype-)| Set the type of  print orientation for the whole workbook. |


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
const { Workbook } = AsposeCells;

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
const { Workbook } = AsposeCells;

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
const { Workbook } = AsposeCells;

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


